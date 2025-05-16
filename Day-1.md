---
title: "Day 1-Introduction To Linux"
seoTitle: "Linux Basics Guide"
seoDescription: "Discover the essentials of Linux: its history, architecture, kernel, and why it's a multi-user, multitasking, open-source operating system"
datePublished: Wed May 14 2025 12:26:04 GMT+0000 (Coordinated Universal Time)
cuid: cmanwzlq1004109jiarr76t6v
slug: day-1-introduction-to-linux
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1747225217255/cabf736d-4ecf-4c06-bd48-e7da126663d5.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1747225344042/f72125b2-4615-4337-8e17-bda18be408f1.png
tags: linux, linux-for-beginners, linux-kernel, linux-basics, linux-commands

---

### **<mark>What is Operating System </mark>** <mark>?</mark>

Operating system is an interface between user and the computer hardware. The hardware of the computer cannot understand the human readable language as it works on binaries i.e. O's and l's. Also it is very tough for humans to understand the binary language, in such case we need an interface which can translate human language to hardware and vice-versa for effective communication.

### **<mark>Types of Operating System:</mark>**

* Single User - Single Tasking Operating System
    
* Single User - Multitasking Operating System
    
* Multi User - Multitasking Operating System
    

1. **Single User - Single Tasking Operating System:-i**n this type of operating system only one user can log into system and can perform only one task at a time.**E.g.: MS-DOs**
    
2. \*\***Single User - Multi tasking operating System**:-\*\*This type of O/S supports only one user to log into the system but a user can perform multiple tasks at a time, browsing internet while playing songs etc.
    
    E.g.: Windows -98,Xp,vista,Seven etc**.**
    
3. \*\***Multi User - Multi Tasking Operating System**:-\*\*These type of O/S provides multiple users to log into the system and also each user can perform various tasks at a time. In a broader term multiple users can logged in to system and share the resources of the system at the same time.
    
    **E.g.: <mark>UNIX, LINUX </mark> etc.**
    

---

**<mark>HISTORY OF LINUX</mark>**

Linus Torvalds had a dream. He wanted to create the coolest operating system in the world that was free for anyone to use and modify. Based on an obscure UNIX flavor called MINIX, Linus took the source code and created his own flavor, called Linux. Using the power of the Internet, he distributed copies of his OS all over the world, and fellow programmers improved upon his work. In 1999, with a dozen versions of the OS and many GUIs to choose from, Linux is causing a UNIX revival. Knowing that people are used to the Windows tools, Linux developers are making applications that combine the best of Windows with the best of UNIX.

**<mark>LINUX PRINICIPLES</mark>**

* Everything is a file:
    
* Small, Single-Purpose Programs
    
* Ability to Chain Programs
    
* Open Source and Free Software
    
* Security and User Privileges
    
* Portability and Multiuser Capability
    
* Multitasking, Stability and Reliability
    
* Community-Driven Development
    

---

* ### **<mark>LINUX ORIGIN</mark>**
    

LINUS TORVALDS

1. a) Finnish college student in 1991
    
2. b) Created Linux Kernel
    
3. When Linux Kernel combined with GNU applications, complete free UNIX like OS was developed.
    

### **<mark>Why Linux?</mark>**

* Fresh implementation of UNIX APIs
    
* Open source development model
    
* Supports wide variety of hardware
    
* Supports many networking protocols and Configurations
    

Fully supported

1. Linux is a UNIX like OS: Linux is a similar to UNIX as the various UNIX versions are to each other.
    
2. Multi-User and Multi-tasking: Linux is a multi-user and multi-tasking operating system. That means that more than one person can be logged on to the same Linux computer at the same time. The same user could even be logged into their account from two or more terminals at the same time; Linux is also Multi-Tasking. A user can have more than one program executing at the same time
    
3. Fully Supported: Red Hat Linux is a fully supported distribution Red Hat Inc. provides many support programs for the smallest to the largest companies.
    

### **<mark>Distributions of Linux (Linux Distros)</mark>**

* A **distribution** is a version of Linux that includes the Linux kernel + software + package manager + user interface.
    

Here are some popular Linux distributions:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1747224497838/43682124-f9c4-4c61-9367-bf5e03a04ef4.png align="center")

---

## **<mark>ARCHITECTURE OF UNIX</mark>**

The architecture of UNIX can be divided into **three levels** of functionality,

1. **KERNEL**
    
2. **SHELL**
    
3. **UTILITY FUNCTIONS**
    

as shown in Figure.

**The lowest level is the kernel,** which schedules tasks, manages resources, and controls security, device management, storage management.

### **1.What is Kernel in Linux?**

The **Kernel** is the **core part of the Linux operating system**.

### ✅ **Functions of the Kernel:**

* **Manages hardware** (CPU, RAM, hard disks, etc.).
    
* **Allocates resources** to programs.
    
* Handles **processes, memory, and device drivers**.
    
* Acts as a **bridge between hardware and software**.
    

📌 You don’t interact directly with the kernel — it works in the background.

**The next level is the shell,** which acts as the user interface, interpreting user commands and starting applications.

## **2.What is Shell in Linux?**

The **Shell** is the **interface between the user and the kernel**.

### ✅ **Functions of the Shell:**

* Takes **commands from the user**.
    
* Sends them to the **kernel** for execution.
    
* Displays the **output** back to the user.
    

There are different types of shells in Linux:

| Shell Name | Description |
| --- | --- |
| **Bash** | Most common shell (Bourne Again Shell) |
| **Sh** | Original Unix shell |
| **Zsh** | Advanced shell with more features |
| **Ksh** | Korn shell, used in scripting |

📌 When you open a terminal and type commands, you're talking to the **shell**.

**3.The highest level is utilities**, which provides utility functions. In other words it is the USER level, as user is the one who operates those utilities.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1747222291839/1aba33f5-9202-4a30-b19d-8405bfb85739.png align="center")

### **<mark>1. File Types in Linux</mark>**

In Linux, **everything is treated as a file** — including directories, hardware devices, and even processes. There are **7 basic file types**:

| **File Type** | **Description** | **Symbol (ls -l)** |
| --- | --- | --- |
| **Regular file** | Normal files containing text, scripts, binary data | `-` |
| **Directory** | A folder that holds other files and directories | `d` |
| **Symbolic link** | Shortcut to another file | `l` |
| **Character device** | Represents devices like keyboard, mouse (char-by-char I/O) | `c` |
| **Block device** | Storage devices like hard drives (block-wise I/O) | `b` |
| **Socket** | For inter-process communication (like a network socket) | `s` |
| **Named pipe (FIFO)** | For communication between processes | `p` |

---

### <mark>Filesystem Hierarchy in Linux (FHS)</mark>

The **Filesystem Hierarchy Standard (FHS)** defines the directory structure and contents in Unix/Linux systems.

Here’s a simplified version of the Linux directory structure:

![Linux File Hierarchy Structure | GeeksforGeeks](https://media.geeksforgeeks.org/wp-content/uploads/20230516105759/151.webp align="left")
