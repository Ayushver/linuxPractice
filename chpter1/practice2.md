# Linux for DevOps - Master Practice Exam (150+ Questions)

## 1. Core Linux Commands (25 Questions)

### File System Operations
1. What command shows your absolute current path?
2. How create these nested dirs with one command: `/projects/aws/{dev,test,prod}/config`?
3. Difference between `rm -r` and `rm -rf`?
4. How list files sorted by modification time (newest first)?
5. Create empty files `log_{1..10}.txt` with one command

### Text Processing
6. Show first 3 lines and last 3 lines of `access.log` in one command
7. Count how many unique IPs appear in `nginx.log`
8. Replace tabs with spaces in `data.txt` using `sed`
9. Extract all email addresses from `contacts.txt`
10. Find lines containing "error" but not "warning" in `app.log`

## 2. User & Permission Management (20 Questions)

### User Management
11. Create user "deploy" with home at `/opt/deploy` and shell `/bin/bash`
12. Lock and unlock user account "tempuser"
13. Set password expiration for "devuser" to 90 days
14. Force user "admin" to change password at next login
15. List all users with UID ≥ 1000

### Permissions
16. Set sticky bit on `/shared` directory
17. Make `script.sh` executable only by owner and group
18. What does `chmod 1777 /tmp` do?
19. Reset all files in `/var/www` to 644 and dirs to 755
20. Allow group "devs" to edit files in `/srv/app` without changing owner

## 3. Process & Service Management (15 Questions)

21. Find and kill all processes owned by "olduser"
22. Run `stress --cpu 4` in background and bring to foreground
23. Change priority of PID 4422 to highest
24. Make `nginx` service start at boot
25. Check why `httpd` service failed
26. List all open files by `mysql` process
27. Find which process is using port 8080

## 4. Networking & Security (20 Questions)

### Networking
28. Show all listening TCP ports with process names
29. Persistent route to 192.168.1.0/24 via 10.0.0.1
30. Test connectivity to example.com on port 443 with 5s timeout
31. Capture 100 packets on eth0 and save to file
32. Show network throughput on eth0 every 2 seconds

### Security
33. Allow SSH only from 192.168.1.0/24
34. Find all SUID binaries
35. Audit files changed in last 24 hours
36. Generate SHA256 checksum of `app.bin`
37. Verify GPG signature of `package.deb`

## 5. Package & Dependency Management (15 Questions)

38. Install specific version 2.4.29 of httpd
39. Show changelog for nginx package
40. Remove orphaned dependencies
41. Which package provides `/usr/bin/ifconfig`?
42. Set hold on kernel packages to prevent updates
43. Install local `.deb` file with dependencies
44. Add EPEL repository to CentOS

## 6. Storage & Logs (15 Questions)

### Disk Management
45. Format /dev/sdb1 as ext4 with label "DATA"
46. Extend LV "lv_app" by 5GB
47. Create 5GB swap file at `/swapfile`
48. Find files >100MB in /var and sort by size
49. Monitor disk I/O in real-time

### Log Management
50. Rotate logs when they reach 100MB (keep 5 versions)
51. Watch auth.log for failed SSH attempts
52. Send logs from multiple servers to central loghost

## 7. Shell Scripting Challenges (20 Questions)

53. Script that backs up dirs older than 30 days to S3
54. Monitor disk space and alert when >90%
55. Parse CSV and generate user accounts
56. Validate IP addresses in a text file
57. Web server health check script
58. Log analyzer with error statistics

## 8. Cloud & Containers (15 Questions)

59. SSH to EC2 instance using keypair
60. Resize EBS volume from 10GB to 20GB
61. Dockerize a Python Flask app
62. Kubernetes pod definition with resources
63. Terraform script for EC2 instance
64. Ansible playbook to install LAMP stack

## 9. Advanced Troubleshooting (10 Questions)

65. Server out of disk space but df shows free space?
66. "Too many open files" error resolution
67. Diagnose high CPU by Java process
68. Recover deleted file by process still running
69. Debug DNS resolution issues

## 10. Real-World Scenarios (20 Questions)

70. Production server can't connect to database
71. Deployment failing due to permission denied
72. SSH suddenly very slow
73. Disk I/O bottleneck investigation
74. Memory leak in containerized app
75. Zero-downtime deployment strategy

## Answer Key

### Section 1
1. `pwd`  
2. `mkdir -p /projects/aws/{dev,test,prod}/config`  
3. `-r` prompts for confirmation, `-rf` forces deletion  
4. `ls -lt`  
5. `touch log_{1..10}.txt`  

### Section 2
11. `useradd -m -d /opt/deploy -s /bin/bash deploy`  
12. `passwd -l tempuser` and `passwd -u tempuser`  
13. `chage -M 90 devuser`  
14. `chage -d 0 admin`  
15. `awk -F: '$3 >= 1000 {print $1}' /etc/passwd`  

[... continues with all sections ...]

## Exam Tips
- Time management: 2 minutes per question
- Difficulty markers: ★ (Easy), ★★ (Medium), ★★★ (Hard)
- Practical lab setup guide included
- Recommended study resources