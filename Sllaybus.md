# Linux for DevOps - Basic Commands Syllabus

## Week 1: Linux Basics & File Operations
**Objective**: Learn fundamental commands for navigating and managing files.

### Shell Basics
- `pwd` (Print Working Directory)
- `ls` (List files)
- `cd` (Change Directory)
- `mkdir` (Make Directory)
- `touch` (Create file)

### File Operations
- `cp` (Copy files)
- `mv` (Move/Rename files)
- `rm` (Remove files)
- `cat` (View file content)
- `less` / `more` (View large files)
- `head` / `tail` (View beginning/end of file)
- `grep` (Search text in files)

**Practice**:
- Navigate directories, create files, and move them
- Search for specific text in log files

## Week 2: File Permissions & User Management
**Objective**: Understand Linux permissions and user roles.

### Permissions
- `chmod` (Change file permissions)
- `chown` (Change file owner)
- `chgrp` (Change group ownership)

### User Management
- `sudo` (Run commands as superuser)
- `useradd` / `usermod` / `userdel` (Manage users)
- `passwd` (Change password)
- `groups` (Check user groups)

**Practice**:
- Create a new user and assign permissions
- Restrict file access to specific users

## Week 3: System Monitoring & Process Management
**Objective**: Learn to monitor system performance and manage processes.

### System Info
- `uname` (System information)
- `df` (Disk space)
- `free` (Memory usage)
- `uptime` (System uptime)

### Process Management
- `ps` (List processes)
- `top` / `htop` (Interactive process viewer)
- `kill` / `pkill` (Terminate processes)
- `systemctl` (Manage system services)

**Practice**:
- Check CPU, memory, and disk usage
- Kill a runaway process

## Week 4: Networking & SSH
**Objective**: Learn networking commands and remote access.

### Network Commands
- `ifconfig` / `ip` (Network interfaces)
- `ping` (Check connectivity)
- `netstat` / `ss` (Network connections)
- `curl` / `wget` (Download files)

### SSH & Remote Access
- `ssh` (Connect to remote servers)
- `scp` (Secure file transfer)
- `rsync` (Efficient file syncing)

**Practice**:
- Transfer files between local and remote machines
- Check open ports on your system

## Week 5: Package Management & Automation
**Objective**: Learn to install software and automate tasks.

### Package Managers
- `apt` (Debian/Ubuntu)
- `yum` / `dnf` (RHEL/CentOS)

### Cron Jobs
- `crontab -e` (Schedule tasks)

### Basic Shell Scripting
- Writing simple `bash` scripts
- Using variables & loops

**Practice**:
- Install a package (e.g., `nginx`)
- Schedule a backup script

## Week 6: DevOps Tools Introduction
**Objective**: Get familiar with essential DevOps tools.

- **Version Control** (`git`)
- **Containers** (`docker` basics)
- **Configuration Management** (`ansible` basics)

**Practice**:
- Clone a Git repository
- Run a simple Docker container

## Final Project
Write a bash script that:
1. Checks disk space
2. Lists top 5 CPU-consuming processes
3. Sends the output to a log file

**Next Steps**:
- Practice daily in a Linux VM (e.g., Ubuntu on VirtualBox)
- Explore advanced topics like `awk`, `sed`, and cloud DevOps tools (AWS/GCP)