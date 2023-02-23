Priority scheduling is a CPU scheduling algorithm where each process is assigned a priority and the process with the highest priority is executed first. In non-preemptive priority scheduling, a process that is currently running cannot be preempted by a process with a higher priority.

Here is a high-level overview of how the priority non-preemptive scheduling algorithm works:

* When a process arrives, its priority is determined (either by the system or by the user).
* The process is added to the ready queue based on its priority.
* The CPU is assigned to the process with the highest priority in the ready queue.
* The process is executed until it completes or is blocked.
* If the process completes, it is removed from the queue.
* If the current process is blocked, it is moved to a blocked queue and the CPU is assigned to the process with the highest priority in the ready queue.
* When a blocked process becomes unblocked (e.g., I/O completes), it is moved back to the ready queue.
* Steps 3-7 are repeated until all processes have completed.

Priority scheduling can be implemented using a variety of data structures, such as a priority queue or a linked list sorted by priority. In non-preemptive priority scheduling, the priority queue is only updated when a new process arrives or when a blocked process becomes unblocked.
