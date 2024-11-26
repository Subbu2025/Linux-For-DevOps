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
