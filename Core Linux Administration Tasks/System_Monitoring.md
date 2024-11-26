## Core Linux Administration Tasks

### 1) Process and System Monitoring
**Tasks:**
1) Monitor running processes using **ps, top, htop, and pidstat**.
2) Manage processes **(kill, pkill, nice, renice, systemctl)**.
3) Check system performance metrics such as CPU, memory, and disk I/O using **vmstat, iostat, and free**.
4) Monitor log files using **tail, head, less, and journalctl**.

1. Monitor Running Processes:
Tools like ps, top, htop, and pidstat help you inspect and monitor processes.
**Example:**
- **View running processes related to Jenkins:**
  ```bash
  ps aux | grep jenkins
  ```
  This shows all processes related to Jenkins, along with their PID and memory usage.

  ![process-example](./images/ps.png)

- **Inspect system-wide process details:**
  ```bash
  top
  ```
  Provides a live view of system processes, along with CPU and memory usage statistics.

  ![top-example](./images/top.png)

- **Use htop for interactive process management:**
  ```bash
  htop
  ```
  - Navigate the process list using arrow keys.
  - Search for Jenkins or Docker processes by pressing / and typing "jenkins" or "docker".

- **Check detailed stats of a specific process:**
  ```bash
  pidstat -p <PID>
  ```
   Replace <PID> with the process ID of Jenkins or Docker to see CPU and memory usage.
  
  **Note:**
  The pidstat command is included in the sysstat package, which might not come pre-installed on your EC2 instance.
  You can install it by following these steps:
  
  - **Amazon Linux / Amazon Linux 2 / RHEL / CentOS:**
  ```bash
  sudo yum install sysstat -y
  ```
   ![pidstat-example](./images/pidstat.png)
