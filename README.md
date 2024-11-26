# Linux Administration Tasks for a DevOps Engineer
**Linux is the backbone of modern-day DevOps, serving as the primary OS for servers, containers, and cloud environments. This guide describes the most important Linux administration tasks with which DevOps engineers must be familiar in order to manage infrastructure effectively and ensure smooth operations of CI/CD pipelines.**
---
## Table of Contents
- [Introduction to Linux Administration in DevOps](#introduction-to-linux-administration-in-devops)

- [Core Linux Administration Tasks](#core-linux-administration)

- [System Monitoring](#system-monitoring)

- [User and Group Management](#user-and-group-management)

- [Package Management](#package-management)

- [File and Directory Management](#file-and-directory-management)

- [Disk and Storage Management](#disk-and-storage)

- [Networking Configuration](#network-configuration)

- [Process and Service Management](#process-and-service-management)

- [Advanced Administration Tasks](#advanced-administration-tasks)

- [Shell Scripting for Automation](#shell-scripting-for-automation)

- [Security Hardening](#security-hardening)

- [Backup and Restore](#backup-and-restore)

- [Log Management](#log-management)

- [Kernel Tuning and Performance Optimization](#kernel-tuning-and-performance-optimization)

- [Practical Real-World Scenarios](#practical-real-world-scenarios)

- [Flowchart Summary and Tips for Interviews](#flowchart-summary-and-tips-for-interviews)
  
---
## 1. Introduction to Linux Administration in DevOps
Linux Administration in the DevOps is mainly related to the management and automation of the Linux system to support applications for deployment, scalability, and reliability. 
Through Linux, DevOps engineers can configure server, host, or deploy containerized applications with system stability support, making it crucial.
## 2. Core Linux Administration Tasks
### I) System Monitoring:

Monitoring ensures the health and performance of Linux servers. Common tools include:

- **top, htop:** View real-time resource usage.

- **vmstat, iostat:** Monitor CPU and I/O statistics.

- **sar:** Collect, report, and save system activity.

- **nmon:** Visualize system metrics like CPU, memory, and network usage.

### II) User and Group Management:
Managing user accounts and permissions is vital to secure multi-user systems.

**Commands:**
- **useradd, usermod, passwd:** Manage users.
  
- **groupadd, gpasswd:** Manage groups.

- **chown, chmod:** Set file permissions.

**Best Practices:**
- Use least-privilege principles.
- Employ sudo for controlled administrative access.

  ### III) Package Management:
  
Linux distributions rely on package managers to install, update, and remove software.

- **Debian-based (e.g., Ubuntu):**
    - Commands: **apt, dpkg**

- **Red Hat-based (e.g., CentOS, RHEL):**
    - Commands: **yum, dnf, rpm**
- Use automation tools like Ansible or Chef for large-scale package management.
  
 ### IV) File and Directory Management:
 
Efficient file management ensures organized and secure systems.

- **Commands:**
  
    - **ls, cd, mkdir, rmdir:** Directory navigation and creation.
  
    - **cp, mv, rm:** File operations.

    - **find, locate, grep:** Search files.

    - **tar, gzip, rsync:** Compress and sync files.

- **Pro Tip:** Use rsync for efficient backup and file transfer.
  
