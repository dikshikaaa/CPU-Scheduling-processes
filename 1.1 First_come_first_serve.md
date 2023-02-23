First-Come, First-Served (FCFS) is a simple CPU scheduling algorithm in which processes are executed in the order in which they arrive. The first process to arrive is the first to be executed, and so on. This algorithm can be implemented using a FIFO (first-in, first-out) queue, which maintains the order of processes based on their arrival time.

Here is a high-level overview of how the FCFS algorithm works:

* When a process arrives, it is added to the end of the ready queue.
* The CPU is assigned to the first process in the queue.
* The process is executed until it completes or is blocked (e.g., waiting for I/O).
* If the process completes, it is removed from the queue.
* If the process is blocked, it is moved to a blocked queue and the CPU is assigned to the next process in the ready queue.
* When the blocked process becomes unblocked (e.g., I/O completes), it is moved back to the ready queue.
* Steps 2-6 are repeated until all processes have completed.
