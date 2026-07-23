# Question 2

## Aim
To create a child process using fork(), monitor its execution from the parent process, terminate it using a signal, and prevent the creation of a zombie process.

## Description
The program uses the fork() system call to create a child process. The parent process waits for a few seconds before sending a SIGTERM signal to terminate the child process. The wait() system call is then used to collect the child's exit status, ensuring that no zombie process is created.
