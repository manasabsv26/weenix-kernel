# weenix-kernel
Documentation and results from my work on the weenix OS kernel

## Setup

Quick instructions for getting Weenix to run on
Redhat-derived or Debian-derived Linux flavors.  

1. Download and install dependencies.

   On recent versions of Ubuntu or Debian, you can simply run:

   $ sudo apt-get install git-core build-essential gcc gdb qemu genisoimage make python python-argparse cscope xterm bash grub xorriso

   or on Redhat:

   $ sudo yum install git-core gcc gdb qemu genisoimage make python python-argparse cscope xterm bash grub2-tools xorriso

2. Compile Weenix:

   $ make

3. Invoke Weenix:

   $ ./weenix -n

   or, to run Weenix under gdb, run:

   $ ./weenix -n -d gdb

To run Weenix under gdb, compilation should be done after setting `GDB_WAIT=1` in Config file

## Weenix Kernel

Developed the core of a small Unix-like operating system. Iteratively implemented:

• Part 1: Threads, Processes, and synchronization primitives
• Part 2: Virtual File System
• Part 3: Virtual Memory and system calls.

1. QEMU terminal
<img src="outputs/images/weenix-welcome.png" alt="QEMU terminal" width="600" />

2. Weenix kernel started with debugger

<img src="outputs/images/kernel-start-with-gdb.png" alt="Weenix kernel started with debugger" width="800" />

3. Sample of kshell, after part 1 of kernel development

<img src="outputs/images/working%20kernel.png" alt="Kshell sample after part 1" width="600" />



