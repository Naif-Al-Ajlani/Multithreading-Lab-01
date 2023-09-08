# Parallel-Computing-Lab-01
 
Multithreading in Python
In Python, the threading module provides a very simple and intuitive API for spawning multiple threads in a program. Let us consider a simple example using a threading module. Let assume we have two threads each calling print_time. This function print the value of the arguments, and date time. 

Threads: 
In computing, a process is an instance of a computer program that is being executed. Any process has 3 basic components:
•	An executable program.
•	The associated data needed by the program (variables, work space, buffers, etc.)
•	The execution context of the program (State of process)

![image](https://github.com/Naif-Al-Ajlani/Parallel-Computing-Lab-01/assets/98528261/416e39d5-f4a9-4286-87ff-c78839d7f8be)


Multiple threads can exist within one process where:
•	A single process may have multiple threads of execution
•	Useful when an application wants to perform many concurrent tasks on shared data
•	Threads share memory and other resources
•	Threads of a process can share the memory of global variables. If a global variable is changed in one thread, this change can be seen by all threads
•	A thread have local (private) variables which can’t be shared by other threads, so any changes in these variables can’t be seen by other threads.
•	Threads often need to coordinate actions through synchronization.
•	Inappropriate synchronization between threads can lead to race conditions problem. 

# Python Example 1:

<img width="450" alt="2023-09-08" src="https://github.com/Naif-Al-Ajlani/Parallel-Computing-Lab-01/assets/98528261/26602fa5-76b9-412c-a949-965474e4bb93">


+ Output
```
I am Thread-1 : Mon Sep  5 13:10:55 2022
I am Thread-1 : Mon Sep  5 13:10:55 2022
I am Thread-2 : Mon Sep  5 13:10:55 2022
I am Thread-1 : Mon Sep  5 13:10:55 2022
I am Thread-2 : Mon Sep  5 13:10:55 2022
I am Thread-1 : Mon Sep  5 13:10:55 2022
I am Thread-2 : Mon Sep  5 13:10:55 2022
I am Thread-1 : Mon Sep  5 13:10:55 2022
I am Thread-2 : Mon Sep  5 13:10:55 2022
I am Thread-2 : Mon Sep  5 13:10:55 2022
Done!
```
# Python Example 2:
Let us consider another example. Let assume we want to start to compute the area of square and rectangle, and volume of cube. Each is different task and don’t depend on each other, so we will create three threads.

<img width="683" alt="2023-09-08 (1)" src="https://github.com/Naif-Al-Ajlani/Parallel-Computing-Lab-01/assets/98528261/e5b4e40c-b01b-456b-a6c4-3cc32c8b601c">

+ Output
```
Square: 100
Rectangle: 50
Cube:  1000
Done!
```

