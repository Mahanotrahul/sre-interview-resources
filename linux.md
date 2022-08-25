1. What is an Operating System? \
Ans: Operating System is a program that acts as an intermediary between a user of a computer and the computer hardware. OS performs all the basic tasks in a computer such as -\
a. file Management \
b. Memory Management \
c. Process Management \
d. Handling I/O \
e. Process Scheduling \
f. Controlling Peripheral devices, etc \

2. What is Process Scheduling? \
Ans: In multi-programming environment, an operating system decides which process gets the processor & for how much time, This is known as process scheduling. OS allocates the processor (CPU) to a process and also de-allocates when a process is no longer required to be run in CPU. \
There are various types of Process Scheduling algorithms that the OS can utilize to schedule the processes. Some of them are -\
a. Round Robin Scheduling \
b. First-Come, First-Serve Scheduling \
c. Shortest Job Next (SJN) \
d. Priority Based Scheduling (PBS) \
In PBS, processes with highest priority is scheduled first. Processes with same priority are scheduled based on FCFS scheduling algorithm.\

3. What is a kernel? \
Ans: Kernel is the one program that runs all the time on the computer. It is the core of a computer's OS with complete control over everything in the system. On most systems, it is one of the first programs loaded on start up (after the boot loader) \
Kernel's interface is a low level abstraction layer. When a process makes requests if the kernel, it is called a system kernel.\

4. What is a BootStrap Program? \
Ans: It is the first code that is executed when the computer system is powered on. The entire OS depends on the bootstrap program to run correctly as it is responsible to load the kernel code into memory and start its execution.

5. What are the type of Process States? \
Ans: A process can have 5 states. \
i. Start: State when a process if first created.\
ii. Ready: State when a process is ready to be assigned to a CPU and executed.\
iii. Running: State when a process is getting executed in the CPU.\
iv. Waiting or Blocked: State when a process is waiting/blocked for a resource to be available.\
v. Terminated/Stopped: State when the process is terminated/stopped.\ 

6. What is System Call? \
Ans: A system call is a controlled entrypoint into the kernel, allowing a process to request that the kernel perform some action on behalf of the process.\
A system aka syscall changes processor state from user mode to kernel mode, so that the CPU can access restricted kernel memory.\
The set of syscakks us fixed and each syscall is identified by a unique number.\

7. What are the steps involved during a syscall? \
Refer to Page 44, Chapter 3 - System Programming Concepts in the book Linux Programming Interface - By Micheal Kerrisk\

8. What are Inodes? \
Ans: A filesystem's inode table contains one i-node for each file in the filesystem. Inodes are identified numerically by their sequential location in the inode table. Each inode is unique for a file and inodes are same for files that are hardlinked to eachother.\
Information contained in an inode:\
i. File Type: regular file, directory, character device, symlink\
ii. Owner: uid\
iii. Group: gid\
iv. Access Permission: permission for three categories of user, owner, group and other.\
v. Three timestamps: time of last access, time of last modification of file and time of last status of change.\
vi. Number of hardlinks to the file.\
vii. Size of the file in the filesystem.\
viii. Number of blocks actually allocated to the file in the filesystem.\
ix. Pointer to data blocks in the filesystem.\
Refer to Section 14.4 - Inodes in Chaper 14 - File Systems in the book Linux Programming Interface - By Micheal Kerrisk

9. What are Boot Block, SuperBlock, Inode Table and Data Blocks? \
Refer to Section 14.3 - Inodes in Chaper 14 - File Systems in the book Linux Programming Interface - By Micheal Kerrisk

10. What is RAID? \
Refer to [Tech Target's article on RAID and RAID controller](https://www.techtarget.com/searchstorage/definition/RAID)

11. Logical Volume Management (LVM)? \
Refer to [OpenSource's Article on LVM](https://opensource.com/business/16/9/linux-users-guide-lvm)

12. Explain Linux Boot Process. \
Refer to [IBM's article on linux Boot Process](https://developer.ibm.com/articles/l-linuxboot/)

13. System Load Average\
Refer to `man uptime`. That's right, mapages to the rescue.

14. Explain various types of Linux Process States? \
Refer to [RedHat's article on Linux process states](https://access.redhat.com/sites/default/files/attachments/processstates_20120831.pdf)

15. Virtualization, Paging, Thrashing\
Refer to [Memory FAQ](https://landley.net/writing/memory-faq.txt)

16. fsync vs fdatasync? \
Some research into this by the developer of Redis - http://oldblog.antirez.com/post/fsync-different-thread-useless.html

17. select vs poll vs epoll? \
Refer to https://hechao.li/2022/01/04/select-vs-poll-vs-epoll/

18. Diff between malloc and calloc? \
Refer to https://www.geeksforgeeks.org/difference-between-malloc-and-calloc-with-examples/

19. Namespaces and cgroups \
Refer to - \
a. https://www.nginx.com/blog/what-are-namespaces-cgroups-how-do-they-work/ \
b. https://jvns.ca/blog/2016/10/10/what-even-is-a-container/
