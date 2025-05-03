# Linux Basic Commands Practice

## 1. Navigation & Directory Inspection

### Find your current location
**Task**: Use the command that shows your present working directory.

### List visible contents
**Task**: List all files and directories in your current folder (non-hidden).

### List all contents (including hidden)
**Task**: List everything in your current directory, including hidden files.

### Navigate to your home directory
**Task**: Change to your home directory using the shortest possible command.

### Go up one directory level
**Task**: Move to the parent directory of your current location.

## 2. Directory Creation

### Create a new directory
**Task**: Make a directory called `test_folder` in your current location.

### Create nested directories
**Task**: Create the path `projects/python/scripts` with a single command (hint: `-p` flag).

## 3. File Operations

### Create an empty file
**Task**: Create a file named `notes.txt` in your current directory.

### Create multiple files at once
**Task**: Create three files: `file1.txt`, `file2.txt`, and `file3.txt` with one command.

### Verify creation
**Task**: List the contents of your directory to confirm the files were created.

## 4. Combined Operations

### Navigate and create
**Task**: Change to your home directory, then create a directory called `temp_work`.

### Create a file inside a new directory
**Task**: First make a directory called `reports`, then create a file `summary.txt` inside it.

### Check your structure
**Task**: From your home directory, list the contents of `temp_work` and `reports` without changing directories (hint: use paths with `ls`).

## 5. Challenge (Optional)
**Task**: Set up this project structure:

# Linux for DevOps - Comprehensive Practice Questions

## Section 1: Linux Fundamentals
1. What command shows your current working directory?
2. How would you list all files (including hidden ones) in a directory?
3. Explain the difference between `cd ~` and `cd ..`
4. Create a nested directory structure `project/src/main/java` with a single command
5. What happens when you run `touch file1 file2 file3`?

## Section 2: File Operations
6. How would you display the last 15 lines of a log file?
7. Create a command that shows lines containing "ERROR" in `system.log`
8. What's the difference between `cat file.txt` and `tac file.txt`?
9. How would you count the number of words in `document.txt`?
10. Write a command to copy `file1.txt` to `backup/file1_copy.txt`

## Section 3: Text Processing
11. Use `sed` to replace all occurrences of "Windows" with "Linux" in `os.txt`
12. How would you delete lines 5-10 from `data.csv` using `sed`?
13. Write a `grep` command to find "404" in all `.log` files in the current directory
14. How would you display only lines that don't contain "DEBUG" in `app.log`?
15. Create a command to show line numbers when displaying `config.txt`

## Section 4: Permissions and Ownership
16. What does `chmod 750 script.sh` do?
17. How would you give the owner full permissions, group read-only, and others no access to `data.db`?
18. Change the owner of `/var/www` to user "webadmin" and group "webgroup"
19. Explain what `rwxr-xr--` permissions mean
20. How would you make `backup.sh` executable for all users?

## Section 5: User and Group Management
21. Create a new user "devuser" with home directory at `/home/dev`
22. Add "devuser" to the "developers" group
23. How would you list all groups a user belongs to?
24. What's the difference between `userdel` and `userdel --remove`?
25. How would you prevent a user from changing their password?

## Section 6: System Administration
26. What command shows disk usage in human-readable format?
27. How would you find all files larger than 100MB in `/var`?
28. Create a command to show running processes sorted by CPU usage
29. How would you schedule a backup script to run daily at 2am?
30. What's the difference between `kill` and `pkill`?

## Section 7: Networking
31. How would you check if port 80 is open on your system?
32. What command downloads a file from `https://example.com/file.zip`?
33. How would you make your Linux server accept password authentication?
34. What's the difference between `ifconfig` and `ip` commands?
35. How would you continuously monitor a growing log file?

## Section 8: Package Management
36. How would you install Git on Ubuntu? On CentOS?
37. What command updates all installed packages on Ubuntu?
38. How would you remove Apache web server but keep its configuration files?
39. Find out which package provides the `ifconfig` command
40. How would you list all installed packages on your system?

## Section 9: Advanced File Operations
41. Create a ZIP archive of `/home/user/documents` called `backup.zip`
42. How would you extract a `.tar.gz` file?
43. Find all `.tmp` files older than 30 days and delete them
44. Search for files named `config.ini` in the entire filesystem
45. How would you compare two text files line by line?

## Section 10: Shell Scripting
46. Write a script that backs up `/var/www` to `/backups` with a timestamp
47. Create a script that monitors disk usage and emails when it's above 90%
48. Write a script that takes a filename as argument and counts its lines
49. Create a script that lists all users who logged in today
50. Write a script that finds duplicate files based on MD5 checksum

## Section 11: VI Editor
51. How do you search for "error" in vi editor?
52. What's the command to save and exit in vi?
53. How would you delete 5 lines in vi?
54. What's the difference between `:wq` and `:x` in vi?
55. How would you undo the last change in vi?

## Section 12: Linux Architecture
56. Name the 4 main components of Linux architecture
57. What's the role of the Linux kernel?
58. Differentiate between Bash and Zsh shells
59. How do system calls work in Linux?
60. What happens when you type `ls -l` and press Enter in terms of Linux architecture?

## Practical Scenarios
61. A server is running out of disk space. Outline your troubleshooting steps
62. How would you give developers write access to `/var/www` without root access?
63. Design a backup strategy for critical configuration files
64. A process is using 100% CPU. How would you identify and resolve it?
65. How would you secure a Linux server for production use?

## Bonus Questions
66. What's the difference between `sudo` and `su`?
67. How would you create a symbolic link to `/usr/bin/python3` called `py`?
68. What command shows the full path of executable programs?
69. How would you run a command in the background?
70. What's the purpose of the `nohup` command?

## Exam Information
- **Total Questions**: 70
- **Question Types**: 
  - Theoretical concepts
  - Practical command writing
  - Scenario-based troubleshooting
  - Scripting challenges
- **Difficulty Levels**:
  - Basic (1-20)
  - Intermediate (21-50)
  - Advanced (51-70)
- **Time Estimate**: 2-3 hours for complete exam

## How to Use This Document
1. Use as a self-assessment tool
2. Practice commands in a Linux VM or container
3. Focus on weak areas identified
4. Time yourself for exam simulation
5. Research concepts you're unfamiliar with

> **Tip**: For hands-on practice, consider setting up an Ubuntu VM or using [Linux containers](https://linuxcontainers.org/) to test your solutions.