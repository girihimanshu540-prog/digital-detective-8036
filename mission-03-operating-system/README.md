# Mission 3 — Understand the Operating System

## 1. Task / objective
Understand the OS .

## 2. Work completed
I under stood the Full function of OS .

### Task 3.1 — Explore my operating system

| Information explored | What it tells you | My observation (privacy-safe) |
|----------------------|-------------------|-------------------------------|
| Operating system / system details (`uname -sr`, `sw_vers`) | Shows which operating system and version my computer runs, and the kernel version | ProductName:		macOS
ProductVersion:		27.2.1
BuildVersion:		26B131 |
| Current account identity (`whoami`) | Shows which user account is currently logged in and running my commands | girihimanshu540 |
| Available and used storage (`df -h`) | Shows how much disk space is in total, how much is used and how much is still free | Filesystem        Size    Used   Avail Capacity iused ifree %iused  Mounted on
/dev/disk3s1s1   926Gi    13Gi   663Gi     2%    487k  4.3G    0%   /
devfs            201Ki   201Ki     0Bi   100%     698     0  100%   /dev
/dev/disk3s6     926Gi    20Ki   663Gi     1%       0  7.0G    0%   /System/Volumes/VM
/dev/disk3s2     926Gi   9.6Gi   663Gi     2%    1.2k  7.0G    0%   /System/Volumes/Preboot
/dev/disk3s4     926Gi    22Mi   663Gi     1%      64  7.0G    0%   /System/Volumes/Update
/dev/disk1s2     550Mi   6.0Mi   531Mi     2%       1  5.4M    0%   /System/Volumes/xarts
/dev/disk1s1     550Mi   6.0Mi   531Mi     2%      47  5.4M    0%   /System/Volumes/iSCPreboot
/dev/disk1s3     550Mi   2.3Mi   531Mi     1%     106  5.4M    0%   /System/Volumes/Hardware
/dev/disk3s5     926Gi   239Gi   663Gi    27%    1.3M  7.0G    0%   /System/Volumes/Data
map auto_home      0Bi     0Bi     0Bi   100%       0     0     -   /System/Volumes/Data/home |
| System activity snapshot (`top`) | Shows a quick view of what the computer is doing right now, such as CPU use, memory use and the busiest processes | PID    COMMAND      %CPU TIME     #TH    #WQ   #PORT MEM    PURG   CMPRS  PGRP  PPID  STATE    BOOSTS          %CPU_ME
14320  top          7.0  00:01.25 1/1    0     28    8752K  0B     0B     14320 14306 running  *0[1]           0.0000 |

### Task 3.2 — Processes
- **What is a process?** A process is a program that is currently running. When I open an app, the operating system starts a process for it.
- **What does the PID column represent?** PID means process identifier. It is a unique number the operating system gives each running process so it can keep track of it.
- **Two examples of processes on my computer:**
  1. (A process you actually saw in the `ps` output, e.g. the browser or editor you opened)
  2. (A second one, e.g. Terminal, or a background system process that you didn't open yourself)

### Task 3.3 — Paths and permissions
- **Absolute vs relative path:**
  - An absolute path starts from the very top of the computer's file system, so it points to the same place no matter where I am. Example from my repo: `/Users/[redacted]/digital-detective-XXXX/mission-03-operating-system/README.md`
  - A relative path starts from the folder I'm currently in. Example from my repo: (write one, e.g. `mission-03-operating-system/README.md` or `../mission-02-terminal`)
- **Permissions of my file (what the owner can do):** drwxr-xr-x@ 3 girihimanshu540  staff    96B Nov 16 00:31 mission-03-operating-system .
Owner can do: read, write, and execute

| Permission | Meaning | Example |
|------------|---------|---------|
| r — Read | Allows the contents of a file to be viewed | Opening a text file to read it |
| w — Write | Allows a file to be changed | Editing and saving a text file |
| x — Execute | Allows a file to be run as a program; on a folder, allows me to enter it | Running a script, or using `cd` to enter a folder |

### Task 3.4 — OS responsibilities

### Task 3.4 — OS responsibilities

| OS responsibility | Your explanation | Example |
|-------------------|------------------|---------|
| Process management | The OS decides which running programs get the CPU and for how long, so many programs can run at the same time. It also starts and stops processes. | Playing music while typing in a document. Both programs keep running because the OS shares CPU time between them. |
| Memory management | The OS gives each program its own share of RAM and takes it back when the program closes, so programs don't overwrite each other's data. | Opening many browser tabs. Each one gets memory, and it is freed when I close the tab. |
| Device management | The OS communicates with hardware like keyboards, printers and pendrives through drivers, so programs don't need to know how each device works. | When I plug in a pendrive, the OS detects it and shows it as a drive I can open. |
| File management | The OS organises how files and folders are named, stored, found, copied, moved and deleted on the storage device. | Saving a document into a folder and finding it again later. |
| User interface / shell | The OS gives me a way to talk to the computer, either through a graphical desktop with windows and icons or through a command-line shell. | Using Terminal commands like `ls`, or clicking icons on the desktop. |
| Security and permissions | The OS controls who can access which files and settings, and protects the system from unauthorised changes. | A file's `rw-` permissions only let its owner read and write it, and a login password stops other people using my account. |

## 3. Commands / tools used
No commands Used .
