# Parallel Computing-Lab-01

Multithreading in Python
In Python, the threading module provides a very simple and intuitive API for spawning multiple threads in a program. Let us consider a simple example using a threading module. Let assume we have two threads each calling print_time. This function print the value of the arguments, and date time. 

# Threads: 
In computing, a process is an instance of a computer program that is being executed. Any process has 3 basic components:
•	An executable program.
•	The associated data needed by the program (variables, work space, buffers, etc.)
•	The execution context of the program (State of process)

![image](https://github.com/Naif-Al-Ajlani/Multithreading-Lab-01/assets/98528261/0a162a5e-0203-4b59-a475-b4e2274f9318)


Multiple threads can exist within one process where:
•	A single process may have multiple threads of execution
•	Useful when an application wants to perform many concurrent tasks on shared data
•	Threads share memory and other resources
•	Threads of a process can share the memory of global variables. If a global variable is changed in one thread, this change can be seen by all threads
•	A thread have local (private) variables which can’t be shared by other threads, so any changes in these variables can’t be seen by other threads.
•	Threads often need to coordinate actions through synchronization.
•	Inappropriate synchronization between threads can lead to race conditions problem. 
