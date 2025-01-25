# linux_from_scratch
**Experimentation and Deployment of Robotic Systems: Course Assignments**  

This repository contains details and work related to the assignments for the course *Experimentation and Deployment of Robotic Systems* under Dr. Daniel M. Aukes. 
The assignments aim to familiarize students with essential tools, terminal commands, and basic system setup required for robotic system experimentation.
This repository showcases a collection of assignments designed to help me learn and practice Linux commands. 
It serves as a beginner-friendly guide to understanding and mastering essential Linux operations.

---

## Assignment 01: System Setup and SSH Key Creation  

**Aim:** Prepare your system for working in this course by installing essential software and demonstrating its functionality.  

### Tasks:  
1. **Virtual Machine Setup**:  
   - Install VirtualBox and the VirtualBox Extension Pack.  
   - Download Ubuntu 22.04 Server Edition (required for ROS2 Humble).  
   - Create a new virtual machine with specifications:  
     - **RAM**: At least 4GB  
     - **Processor**: At least 1 (2 recommended)  
     - **Hard Drive**: 50GB dynamically allocated in `.vdi` format  
     - **USB Controller**: USB 3.0  
     - **Network**: Bridged network adapter  
     - **Shared Folder**: Accessible between host OS and VM  

2. **Ubuntu Installation**:  
   - Install Ubuntu 22.04 on the virtual machine.  
   - Take a snapshot of the terminal in GNOME with the machine name updated to include your ASURITE ID.  

3. **SSH Key Creation**:  
   - Generate an **ed25519 private key** and save it in the `~/.ssh` folder.  
   - Copy the public key to the VirtualBox shared folder or your host machine.  

4. **Tailscale Setup**:  
   - Create a Tailscale account.  
   - Install Tailscale on the virtual machine and register it with your account.  
   - Disable key expiry and verify the machine registration using `tailscale status`.  
   - Ping the device to ensure connectivity and take a screenshot of the result.

---

## Assignment 02: Introduction to Terminal Commands  

**Aim:** Practice terminal commands, filesystem navigation, file handling, and process management in a controlled SSH session.  

### Tasks:  

1. **SSH Session Setup**:  
   - Log in to the provided hostname using your ASURITE username and the private key created in Assignment 01.  
   - Save your session using the `script` command for logging all activities.  

2. **File System Navigation**:  
   - Navigate to different directories and list files with specific patterns.  
   - Answer conceptual questions (e.g., the behavior of `cd` without arguments) by echoing responses.  

3. **File Search and Grep**:  
   - Locate files with specific extensions or starting characters.  
   - Use `grep` to search for specific strings within files and display matching lines with line numbers.  

4. **File and Directory Creation**:  
   - Create a nested directory structure using `mkdir`.  
   - Write, append, and manipulate file content using commands like `>`, `>>`, and `touch`.  

5. **Advanced Functions**:  
   - Show the total disk usage of a directory.  
   - Replace words within files using terminal commands (e.g., replace "stew" with "pot").  

6. **Variables**:  
   - Create, display, and export variables.  
   - Identify environment variables in the session.  

7. **Process Management**:  
   - Launch a subprocess with `sleep infinity`.  
   - Identify the process ID (PID) and terminate it.  

8. **Submission**:  
   - Copy and paste the session log to a text editor and submit the complete session for review.  

---

**Note:** These assignments provide hands-on practice for mastering terminal operations, SSH sessions, and system management—critical skills for deploying robotic systems efficiently.  

Feel free to explore each assignment in detail within the repository.  
