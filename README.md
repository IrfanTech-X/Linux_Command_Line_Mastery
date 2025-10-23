# 🐧 Linux Command Line Mastery

Welcome to **Linux Command Line Mastery** — your all-in-one guide to learning, understanding, and mastering the Linux terminal.  
This repository contains **300+ essential Linux commands**, organized by category with simple explanations and examples.  

---

## 📖 About This Repository
The Linux command line is powerful — mastering it opens doors to automation, development, and system administration.  
This project helps students, developers, and enthusiasts strengthen their Linux skills through hands-on command examples.

---
## 🧑‍💻 Change Username (Recommended - Simple)

### ⏱ Step-by-Step (Takes 2–3 Minutes)

Run these commands one by one in your **Terminal** (`Ctrl + Alt + T`):

### ⚙️ Step-by-Step Guide

| Step | Description | Command |
|------|--------------|----------|
| **1** | **Login as Root 👑** | `sudo -i` |
| **2** | **Change Username** | `sudo usermod -l NEW_USERNAME -d /home/NEW_USERNAME -m OLD_USERNAME` |
| **3** | **(Optional) Change Group Name** | `sudo groupmod -n NEW_USERNAME OLD_USERNAME` |
| **4** | **Fix Ownership** | `sudo chown -R NEW_USERNAME:NEW_USERNAME /home/NEW_USERNAME` |
| **5** | **Reboots the system to apply all changes** | `sudo reboot` |

💡 **Tip:**  
Replace `OLDNAME` with your **current username** and `NEWNAME` with your **desired new username**.

---

## 🗂️ Command Categories

| Category | Description |
|-----------|-------------|
| 🧭 **Navigation & File Management** | Move around directories and manage files |
| ⚙️ **System Information** | Learn about your system’s hardware and performance |
| 🔐 **User Management** | Manage users, groups, and permissions |
| 📦 **Package Management** | Install, update, and remove software |
| 🌐 **Networking** | Configure and test network connections |
| 🧰 **Process Control** | Manage running processes and system resources |
| 📝 **File Editing & Viewing** | Edit, view, and analyze text files |
| 🖥️ **Disk Management** | Manage storage devices and usage |
| 🚀 **Shortcuts & Tricks** | Speed up your workflow with quick commands |

---

## 💡 Example Commands

## 🔐 User Management

| Command | Description | Example |
|----------|-------------|----------|
| `whoami` | Shows the **username** of the currently logged-in user. | `whoami` |
| `id` | Displays your **user ID, group ID, and permissions**. | `id` |
| `adduser` | Creates a **new user account** and home directory. | `sudo adduser irfan` |
| `passwd` | Changes the **password** for a user account. | `passwd` |
| `su` | Switches to another user (commonly used to switch to root). | `su root` |
| `groups` | Lists all **groups** a user belongs to. | `groups irfan` |
| `chmod` | **Changes file permissions** (read, write, execute). | `chmod 755 script.sh` |
| `chown` | Changes the **ownership** of files or directories. | `sudo chown irfan file.txt` |

💬 **Tip:** `chmod +x filename.sh` makes a script executable.

---

## 🌐 Networking

| Command | Description | Example |
|----------|-------------|----------|
| `ping` | Sends packets to another host to **test network connectivity**. | `ping google.com` |
| `ifconfig` | Displays **network interfaces** and IP addresses. | `ifconfig` |
| `ip addr` | Shows detailed **IP configuration**. | `ip addr show` |
| `netstat -tuln` | Displays all **active network connections** and listening ports. | `netstat -tuln` |
| `curl` | Transfers data from a URL; great for testing APIs or downloading small files. | `curl https://example.com` |
| `wget` | Downloads files from the internet. | `wget https://example.com/file.zip` |
| `traceroute` | Tracks the **path packets take** to reach a destination host. | `traceroute google.com` |
| `nslookup` | Looks up DNS information for a domain. | `nslookup google.com` |

💬 **Tip:** Use `ping -c 4 google.com` to send exactly 4 packets instead of pinging forever.

---
## 🧭 Navigation & File Management

| Command | Description | Example |
|----------|-------------|----------|
| `pwd` | Displays the full path of your **current working directory**, helping you know your exact location in the system. | `pwd` |
| `ls` | Lists all **files and directories** in the current folder. Add `-l` for detailed info or `-a` to show hidden files. | `ls -la` |
| `cd` | Changes the **current directory**. Use `cd ..` to move up one level or `cd ~` to go back to your home folder. | `cd /home/user/Documents` |
| `mkdir` | Creates a **new directory (folder)** at the specified path. | `mkdir projects` |
| `rmdir` | Removes an **empty directory**. It won’t delete folders that contain files. | `rmdir old_folder` |
| `cp` | **Copies** files or directories from one location to another. Use `-r` to copy folders recursively. | `cp file.txt /backup/` |
| `mv` | **Moves or renames** files or directories. | `mv notes.txt Documents/` |
| `rm` | **Deletes** files or directories. Use `-r` for recursive delete and `-f` to force deletion. |`rm -rf test_folder` `rm file.txt` |
| `touch` | Creates a **new empty file** or updates a file’s modification timestamp. | `touch newfile.txt` |
| `cat` | **Displays file contents** directly in the terminal. Great for reading small text files. | `cat notes.txt` |
| `less` | Opens a file **page by page**, allowing you to scroll with arrows or spacebar. | `less logfile.log` |
| `more` | Similar to `less`, but moves forward one screen at a time. | `more text.txt` |
| `head` | Displays the **first 10 lines** of a file (default). Add `-n` to specify a custom number. | `head -n 5 file.txt` |
| `tail` | Shows the **last 10 lines** of a file. Use `-f` to monitor logs in real time. | `tail -f syslog` |
| `tree` | Displays all files and folders in a **tree-like structure**. | `tree /home/user` |
| `find` | **Searches for files or directories** by name or pattern within a path. | `find /home -name "*.txt"` |
| `locate` | Quickly **finds files** using a prebuilt system index. Run `updatedb` first if needed. | `locate config.json` |
| `which` | Shows the **full path** of a command or executable. | `which python` |
| `whereis` | Locates the **binary, source, and man page** files for a command. | `whereis ls` |
| `echo` | Prints text or variable output to the terminal. | `echo "Hello Linux"` |
| `cat > file` | Creates a **new file** and lets you type its content directly in the terminal. Press `Ctrl + D` to save and exit. | `cat > note.txt` | 
|  |**If used again on the same file, it will overwrite the existing content.** | `cat > note.txt` |
| `cat >> file` | **Appends** new content to an existing file without deleting previous data. Press `Ctrl + D` to save and exit. | `cat >> note.txt` |
| `cat file1 file2 > newfile` | Combines multiple files into one. | `cat a.txt b.txt > combined.txt` |
| `grep` | Searches for **specific text patterns** inside files. | `grep "error" logfile.log` |
| `sort` | **Sorts lines** in a file alphabetically or numerically. | `sort names.txt` |
| `uniq` | Removes consecutive **duplicate lines** from a sorted file. | `uniq sorted.txt` |
| `wc` | Displays **number of lines, words, and bytes/characters** in a file. | `wc file.txt` |
| `diff` | Compares two text files **line by line** and shows the differences. | `diff file1.txt file2.txt` |
| `cmp` | Compares two files **byte by byte** to check for differences. | `cmp image1.jpg image2.jpg` |
| `file` | Displays the **type of file**, such as text, binary, or executable. | `file script.sh` |
| `basename` | Extracts the **filename** from a full path. | `basename /home/user/file.txt` |
| `dirname` | Extracts the **directory path** from a file path. | `dirname /home/user/file.txt` |
| `du` | Shows **disk usage** of files and directories. Use `-h` for human-readable sizes. | `du -sh *` |
| `df` | Displays **disk space usage** of all mounted filesystems. | `df -h` |
| `ln` | Creates **hard or symbolic links** between files. | `ln -s file.txt shortcut.txt` |
| `history` | Displays a **list of recently used commands** in the current shell. | `history` |
| `clear` | **Clears the terminal screen**, keeping it tidy. | `clear` |
| `alias` | Creates a **shortcut command** for a long command sequence. | `alias ll='ls -la'` |
| `unalias` | Removes a previously defined alias. | `unalias ll` |
| `man` | Opens the **manual (help) page** for any Linux command. | `man ls` |
| `whoami` | Displays the **current logged-in username**. | `whoami` |
| `hostname` | Shows or sets the **system’s hostname**. | `hostname` |
| `date` | Displays or sets the **current date and time**. | `date` |
| `cal` | Displays a **calendar** for the current or specified month/year. | `cal 2025` |
| `uptime` | Shows how long the **system has been running** and load averages. | `uptime` |
| `lsblk` | Lists all **block storage devices** like hard drives or USBs. | `lsblk` |
| `stat` | Displays detailed **file metadata** such as size, permissions, and timestamps. | `stat file.txt` |
| `xargs` | Builds and executes commands using **input from another command**. | `find . -name "*.txt" \| xargs rm` |
| `cut` | Extracts **specific fields or columns** from a line of text. | `cut -d ':' -f1 /etc/passwd` |
| `paste` | **Merges lines** from multiple files side by side. | `paste file1 file2` |
| `tee` | Writes output to **both a file and the screen simultaneously**. | `ls | tee list.txt` |

💬 **Tip:** To quickly check what’s inside your folder, use `ls -lh` to see file sizes in a human-readable format and `ls -lt` to sort by modification time.
---
## 🔍 Searching & Acting on Files with `find` and `xargs`

| Command | Description | Example |
|----------|-------------|----------|
| `find` | Searches for **files or directories** in a specified location using name patterns, type, size, or other criteria. | `find . -name "*.txt"` |
| `find` | Searches for a **specific file** in a given directory. | `find /home -name "note.txt"` |
| `xargs` | Builds and executes commands using **input from another command**. Useful for performing actions on multiple files. | `find . -name "*.txt" | xargs rm` |
| `xargs` | Combine `find` and `xargs` to process files efficiently, like viewing or editing multiple files at once. | `find /home -name "*.log" | xargs cat` |

💡 **Tips:**  
- `.` → current directory, `/home` → specific folder.  
- Always use quotes with wildcards, e.g., `"*.txt"`.  
- You can replace `rm` or `cat` in `xargs` with any other command, like `mv` or `chmod`.  
- For safer deletion, first run:  
  ```bash
  find . -name "*.txt" | xargs echo
---
## 📂 Sorting and Removing Duplicates with `sort` & `uniq`

| Command | Description | Example |
|---------|-------------|---------|
| `sort` | **Sorts lines** in a file alphabetically or numerically. | `sort names.txt` |
| `sort -u` | **Sorts lines and removes duplicates** in one step. | `sort -u file.txt` |
| `uniq` | Removes consecutive **duplicate lines** from a sorted file. | `uniq sorted.txt` |
| `sort file.txt \| uniq` | **Sorts the file** and then removes all duplicates. | `sort names.txt \| uniq` |
| `sort file.txt \| uniq -c` | **Counts occurrences** of each line after sorting. | `sort names.txt \| uniq -c` |
| `sort file.txt \| uniq -d` | Shows only **duplicate lines** after sorting. | `sort names.txt \| uniq -d` |
| `sort file.txt \| uniq -u` | Shows only **unique (non-repeated) lines** after sorting. | `sort names.txt \| uniq -u` |
| `sort -f file.txt \| uniq -i` | Ignores **case differences** when sorting and removing duplicates. | `sort -f names.txt \| uniq -i` |

💡 **Tips:**  
- Always use `sort` before `uniq` if duplicates are **not consecutive**.  
- Combine with `grep` to filter specific patterns before removing duplicates:  
  ```bash
  grep "error" log.txt | sort | uniq -c

---
## 📊 File Count Analysis with `wc`

| Command | Description | Example |
|---------|-------------|---------|
| `wc` | Displays **number of lines, words, and bytes** in a file. | `wc file.txt` |
| `wc -l` | Shows only the **number of lines** in a file. | `wc -l file.txt` |
| `wc -w` | Shows only the **number of words** in a file. | `wc -w file.txt` |
| `wc -c` | Shows only the **number of bytes** in a file. | `wc -c file.txt` |
| `wc -m` | Shows only the **number of characters** in a file (useful for multibyte text). | `wc -m file.txt` |
| `wc -L` | Displays the **length of the longest line** in a file. | `wc -L file.txt` |
| `wc file1.txt file2.txt` | Shows counts for **multiple files** and a total at the bottom. | `wc file1.txt file2.txt` |
| `cat file.txt \| wc -l` | Counts the **number of lines** in a file using a pipe. | `cat file.txt | wc -l` |
| `cat file.txt \| wc -w` | Counts the **number of words** in a file using a pipe. | `cat file.txt | wc -w` |

💡 **Tips:**  
- Use `wc -m` instead of `-c` if your file contains **Unicode or multibyte characters**, to get an accurate character count.  
- Combine with `sort` or `grep` to count specific lines or patterns:  
  ```bash
  grep "error" log.txt | wc -l

---
## 📂 Directory Navigation with `cd`

| Command | Description | Example |
|----------|-------------|----------|
| `cd` | Changes the **current directory**. If used alone, it takes you to your **home directory**. | `cd` |
| `cd ~` | Quickly jumps to your **home directory** (same as just typing `cd`). | `cd ~` |
| `cd ..` | Moves **one level up** from the current directory (to the parent folder). | `cd ..` |
| `cd /` | Takes you to the **root directory** of the Linux filesystem. | `cd /` |
| `cd -` | Switches back to the **previous directory** you were in. | `cd -` |
| `cd /path/to/folder` | Moves directly to the specified directory path. | `cd /home/user/Documents` |
| `cd ../..` | Moves **two levels up** in the directory structure. | `cd ../..` |
| `cd ~/Downloads` | Moves to the **Downloads folder** inside your home directory. | `cd ~/Downloads` |
| `cd "$(dirname FILE)"` | Changes to the **directory containing a specific file**. | `cd "$(dirname script.sh)"` |

💡 **Tips:**  
- Use `pwd` after `cd` to confirm your current directory.  
- Combine `cd` with `ls` to explore directories efficiently:  
  ```bash
  cd /etc && ls

---
## ✏️ Editing Files with Nano

| Command | Description | Example |
|----------|-------------|----------|
| `nano` | Opens the **Nano text editor** directly in the terminal. It’s simple and beginner-friendly for editing text files. | `nano file.txt` |

### 🧭 Basic Nano Shortcuts

| Shortcut | Action |
|-----------|---------|
| `Ctrl + O` then `Enter` | Save changes (Write Out) |
| `Ctrl + X` | Exit Nano |
| `Ctrl + G` | Show help |
| `Ctrl + K` | Cut a line |
| `Ctrl + U` | Paste a line |
| `Ctrl + W` | Search text |
| `Ctrl + C` | Show cursor position |

💡 **Tip:**  
If the file doesn’t exist, `nano` will automatically create it when you save.  
Example:  
```bash
nano notes.txt
```
---

## ⚙️ System Information

| Command | Description | Example |
|----------|-------------|----------|
| `uname -a` | Shows **complete system and kernel details**, including OS name, version, and architecture. | `uname -a` |
| `lscpu` | Displays **CPU architecture and core details**. | `lscpu` |
| `lsmem` | Lists **system memory blocks and sizes**. | `lsmem` |
| `lsusb` | Shows information about **USB devices** connected. | `lsusb` |
| `lspci` | Lists **PCI devices** such as network and sound cards. | `lspci` |
| `lsmod` | Displays **loaded kernel modules**. | `lsmod` |
| `hostnamectl` | Shows or changes the **system hostname and related info**. | `hostnamectl` |
| `uptime` | Shows **system uptime**/Tells you **how long your system has been running** and the average CPU load. | `uptime` |
| `top` | Displays a **live view of all running processes**, their resource usage(CPU/memory usage), and system load. | `top` |
| `htop` | An improved, **interactive colorful version** of `top` with interactive process control. | `htop` |
| `free -m` | Displays **memory usage** (RAM and swap) in megabytes. | `free -m` |
| `free -h` | Displays **RAM and swap usage** in human-readable format. | `free -h` |
| `vmstat` | Reports **virtual memory statistics**. | `vmstat 2 5` |
| `iostat` | Displays **CPU and device I/O statistics**. | `iostat` |
| `df -h` | Shows **disk space usage** of filesystems. | `df -h` |
| `du -sh` | Displays **total size** of a directory. | `du -sh /home/user` |
| `who` | Lists all **currently logged-in users**. | `who` |
| `w` | Shows **who is logged in** and what they’re doing. | `w` |
| `last` | Displays **login history**. | `last` |
| `id` | Prints **user and group IDs**. | `id` |
| `groups` | Lists **groups** a user belongs to. | `groups user` |
| `lsb_release -a` | Prints **Linux distribution info**. | `lsb_release -a` |
| `dmesg` | Displays **kernel ring buffer messages**, useful for troubleshooting hardware. | `dmesg | less` |
| `lsof` | Lists **open files and the processes** using them. | `lsof` |
| `ps aux` | Shows **all running processes** in detail. | `ps aux` |
| `env` | Displays all **environment variables**. | `env` |
| `printenv` | Prints the value of a specific environment variable. | `printenv PATH` |
| `set` | Displays or modifies **shell variables**. | `set` |
| `export` | Makes a variable **available to child processes**. | `export PATH=$PATH:/opt/bin` |
| `uname -r` | Shows the **kernel release version**. | `uname -r` |
| `uptime -p` | Prints uptime in **pretty format** (e.g., “up 2 hours, 5 minutes”). | `uptime -p` |
| `whoami` | Displays **current username**. | `whoami` |
| `hostname` | Prints **system hostname** (the name your machine is identified by on a network). | `hostname` |
| `arch` | Displays **machine architecture** (e.g., x86_64). | `arch` |
| `dmidecode` | Displays **hardware information** from the system BIOS. | `sudo dmidecode -t system` |
| `inxi` | Displays **comprehensive hardware info** in readable format. | `inxi -Fxz` |
| `uptime -s` | Shows the **exact system boot time**. | `uptime -s` |
| `date` | Prints the **current date and time**. | `date` |
| `cal` | Displays a **monthly calendar** right in the terminal. | `cal` |
| `neofetch` | Shows a **summary of OS and hardware info** with a nice logo. | `neofetch` |

💬 **Tip:** Use `watch -n 1 free -m` to continuously monitor memory usage every second.

---

## 💻 Process & Job Management

| Command | Description | Example |
|----------|-------------|----------|
| `ps` | Shows **snapshot of running processes**. | `ps aux` |
| `pstree` | Displays processes in a **tree view**. | `pstree` |
| `pgrep` | Finds processes by **name pattern**. | `pgrep firefox` |
| `pidof` | Displays the **PID (process ID)** of a running program. | `pidof sshd` |
| `kill` | Sends a **signal to terminate** a process by PID. | `kill 1234` |
| `killall` | Kills **all processes** with a given name. | `killall firefox` |
| `pkill` | Sends signal to processes **matching name/pattern**. | `pkill -f chrome` |
| `jobs` | Lists all **background jobs** in the current session. | `jobs` |
| `bg` | **Resumes** a suspended job in the background. | `bg %1` |
| `fg` | Brings a **background job to the foreground**. | `fg %1` |
| `nice` | Starts a process with a **modified scheduling priority**. | `nice -n 10 script.sh` |
| `renice` | Changes the **priority** of an existing process. | `renice 5 -p 2345` |
| `top` | Displays **real-time process activity**. | `top` |
| `htop` | Interactive viewer for processes. | `htop` |
| `at` | Schedules a command to **run once at a specific time**. | `echo "backup.sh" | at 23:00` |
| `batch` | Queues jobs to **run when system load is low**. | `echo "update.sh" | batch` |
| `cron` | Runs scheduled tasks **at fixed times**. | `crontab -e` |
| `crontab -l` | Lists the **current user’s cron jobs**. | `crontab -l` |
| `service` | Starts/stops/manages **system services**. | `sudo service apache2 restart` |
| `systemctl` | Controls **systemd services and units**. | `sudo systemctl status nginx` |
| `nohup` | Runs a command **immune to hangups**, continuing after logout. | `nohup script.sh &` |
| `disown` | Removes a job from the shell’s job table so it won’t terminate when the shell exits. | `disown %1` |
| `time` | Measures **execution time** of a command. | `time ls -R /` |
| `watch` | Repeats a command **at regular intervals**, showing output changes. | `watch -n 5 df -h` |
| `strace` | Traces **system calls and signals** of a process. | `strace -p 1234` |
| `lsof -p` | Lists **files opened by a specific PID**. | `lsof -p 1234` |
| `uptime` | Shows system uptime and load averages. | `uptime` |
| `pidstat` | Reports **statistics for specific processes**. | `pidstat 1` |
| `systemctl list-units` | Lists all **active systemd units/services**. | `systemctl list-units` |
| `systemctl enable` | Enables a service to **start on boot**. | `sudo systemctl enable nginx` |
| `systemctl disable` | Disables a service from starting automatically. | `sudo systemctl disable nginx` |
| `systemctl stop` | Stops a running service. | `sudo systemctl stop ssh` |
| `systemctl start` | Starts a service manually. | `sudo systemctl start ssh` |
| `systemctl restart` | Restarts a service. | `sudo systemctl restart ssh` |
| `journalctl` | Views **systemd logs**. | `journalctl -xe` |
| `top -u` | Shows processes belonging to a **specific user**. | `top -u student` |
| `pkexec` | Runs commands as another user (like GUI sudo). | `pkexec gedit` |
| `uptime -p` | Shows uptime in human-readable format. | `uptime -p` |
| `ps -eo pid,ppid,cmd,%mem,%cpu` | Displays extended **process info with CPU and memory usage**. | `ps -eo pid,cmd,%mem,%cpu` |

💬 **Tip:** Use `top`, `htop`, and `pidstat` together to track both system-wide and per-process resource usage.

---
## 🌐 Networking Commands

| Command | Description | Example |
|----------|-------------|----------|
| `ifconfig` | Displays or configures **network interfaces** (use `ip addr` in modern systems). | `ifconfig` |
| `ip addr` | Shows **IP addresses and network interfaces** on your system. | `ip addr` |
| `ping` | Sends **ICMP packets** to check connectivity to a host. | `ping google.com` |
| `traceroute` | Shows the **path packets take** to reach a host. | `traceroute google.com` |
| `netstat` | Displays **network connections, routing tables, and interface stats**. | `netstat -tuln` |
| `ss` | Modern alternative to `netstat`, shows **socket statistics**. | `ss -tulw` |
| `wget` | Downloads **files from the internet** via command line. | `wget https://example.com/file.txt` |
| `curl` | Transfers data to/from a server. Can **fetch web pages** or send requests. | `curl https://example.com` |
| `scp` | **Copies files securely** between hosts over SSH. | `scp file.txt user@remote:/home/user/` |
| `rsync` | Efficiently **syncs files** between local and remote systems. | `rsync -av file.txt user@remote:/home/user/` |
| `ftp` | Connects to a **remote FTP server** to transfer files. | `ftp ftp.example.com` |
| `sftp` | Secure FTP over SSH for **encrypted file transfer**. | `sftp user@remote` |
| `ssh` | Connects to a **remote server securely** using SSH. | `ssh user@server.com` |
| `hostname` | Displays or sets the **system hostname**. | `hostname` |
| `dig` | Performs **DNS lookups** and shows detailed DNS info. | `dig example.com` |
| `nslookup` | Queries **DNS to resolve domain names** to IPs. | `nslookup google.com` |
| `route` | Displays or manipulates the **IP routing table**. | `route -n` |
| `arp` | Shows the **ARP cache** mapping IP addresses to MAC addresses. | `arp -a` |
| `curl -I` | Fetches **HTTP headers** of a webpage. | `curl -I https://example.com` |
| `tcpdump` | Captures and analyzes **network packets** in real time. | `sudo tcpdump -i eth0` |
| `nmap` | Scans **network hosts and ports**. | `nmap 192.168.1.1` |
| `ethtool` | Displays or configures **network interface parameters**. | `ethtool eth0` |
| `ping6` | Sends **ICMP packets for IPv6 connectivity**. | `ping6 google.com` |
| `iwconfig` | Shows or configures **wireless network interfaces**. | `iwconfig wlan0` |
| `nmcli` | Command-line tool for **NetworkManager** to manage network connections. | `nmcli device status` |
| `curl -O` | Downloads a **file from a URL** and saves it with the same name. | `curl -O https://example.com/file.txt` |
| `wget -c` | **Continues an interrupted download** from where it left off. | `wget -c file.zip` |
| `scp -r` | Recursively copies **directories over SSH**. | `scp -r folder user@host:/path` |
| `rsync --delete` | Syncs directories and **removes extra files** from the destination. | `rsync -av --delete source/ dest/` |
| `dig +short` | Quickly returns the **IP address** of a domain. | `dig +short example.com` |
| `who` | Lists **users currently logged in**. | `who` |
| `w` | Displays **logged-in users and their current activity**. | `w` |
| `finger` | Shows detailed info about a **user**. | `finger username` |
| `uptime` | Shows **system running time and load averages**. | `uptime` |
| `netcat` | Reads and writes data over network connections; useful for **port testing**. | `nc -zv host 80` |
| `hostnamectl` | Displays or **sets hostname and OS info**. | `hostnamectl status` |
| `ip route` | Shows **routing table** for network traffic. | `ip route` |
| `systemctl status network` | Shows the **network service status** on systemd-based systems. | `systemctl status NetworkManager` |
| `ping -c 5` | Sends a limited number of **ping requests**. | `ping -c 5 example.com` |
| `ss -tulpn` | Shows **listening sockets** with process info. | `ss -tulpn` |
| `traceroute -6` | Traces **IPv6 route** to a destination. | `traceroute -6 example.com` |
| `iptables -L` | Lists **firewall rules** in iptables. | `sudo iptables -L` |
| `ufw status` | Displays the **status of UFW firewall**. | `sudo ufw status` |
| `iptables -A INPUT -p tcp --dport 22 -j ACCEPT` | Adds a **firewall rule** to allow SSH traffic. | `sudo iptables -A INPUT -p tcp --dport 22 -j ACCEPT` |
| `ping -i 0.5` | Sends **ping packets at 0.5s interval**. | `ping -i 0.5 google.com` |
| `curl -L` | Follows **HTTP redirects** while fetching a URL. | `curl -L https://example.com` |
| `wget -q` | Downloads a file **quietly** without showing progress. | `wget -q file.zip` |
| `scp -P` | Uses a **custom port** for SSH file transfer. | `scp -P 2222 file.txt user@host:/path` |
| `rsync -z` | Enables **compression during sync** to save bandwidth. | `rsync -avz source/ dest/` |
| `netstat -anp` | Shows all **connections and listening ports** with process info. | `netstat -anp` |
| `curl -I -L` | Fetches **headers and follows redirects**. | `curl -I -L https://example.com` |
| `ping -s 64` | Sends a **custom-size ping packet**. | `ping -s 64 google.com` |
| `dig MX` | Shows **mail exchange (MX) records** of a domain. | `dig MX example.com` |
| `nslookup -type=MX` | Alternative way to get **MX records**. | `nslookup -type=MX example.com` |
| `traceroute -n` | Shows **IP addresses only** in the route. | `traceroute -n example.com` |
| `arp -a` | Lists **all cached ARP entries**. | `arp -a` |
| `ip link set eth0 up` | Brings a **network interface up**. | `ip link set eth0 up` |
| `ip link set eth0 down` | Brings a **network interface down**. | `ip link set eth0 down` |

💬 **Tip:** For network troubleshooting, combine `ping`, `traceroute`, and `nslookup` for faster diagnosis.

---

## 🔒 File Permissions & Ownership

| Command | Description | Example |
|----------|-------------|----------|
| `chmod` | Changes **file or directory permissions** (read, write, execute). | `chmod 755 script.sh` |
| `chown` | Changes **owner and group** of a file or directory. | `chown user:group file.txt` |
| `chgrp` | Changes **group ownership** of a file or directory. | `chgrp staff file.txt` |
| `umask` | Shows or sets the **default file creation permissions**. | `umask 022` |
| `ls -l` | Displays **detailed file info** including permissions, owner, and group. | `ls -l` |
| `stat` | Displays detailed **file metadata**, including permissions and timestamps. | `stat file.txt` |
| `getfacl` | Displays **access control list (ACL)** for a file. | `getfacl file.txt` |
| `setfacl` | Sets **ACL permissions** for a file. | `setfacl -m u:user:rwx file.txt` |
| `umask 077` | Restricts **default permissions** for new files to owner only. | `umask 077` |
| `chmod -R 700` | Recursively sets **permissions** for all files in a directory. | `chmod -R 700 project/` |
| `chown -R user:group` | Changes **owner/group recursively** for a folder. | `chown -R user:staff project/` |
| `touch file.txt` | Creates a file with **default permissions** based on umask. | `touch file.txt` |
| `ls -la` | Shows **all files including hidden ones** with detailed info. | `ls -la` |
| `whoami` | Shows the **current user**, helpful when managing permissions. | `whoami` |
| `groups` | Shows **groups** the current user belongs to. | `groups` |
| `id` | Displays **user ID, group ID, and group memberships**. | `id` |
| `sudo` | Executes a command **with administrative privileges**. | `sudo apt update` |
| `su` | Switches to another user (root by default). | `su -` |
| `sudo -i` | Opens a **root shell**. | `sudo -i` |
| `chmod u+x file.sh` | Gives **execute permission** to the file owner. | `chmod u+x script.sh` |
| `chmod g-w file.txt` | Removes **write permission** for the group. | `chmod g-w file.txt` |
| `chmod o-r file.txt` | Removes **read permission** for others. | `chmod o-r file.txt` |
| `lsattr` | Shows **file attributes**, e.g., immutable flag. | `lsattr file.txt` |
| `chattr +i` | Makes a file **immutable** (cannot be deleted/modified). | `chattr +i important.txt` |
| `chattr -i` | Removes **immutable attribute**. | `chattr -i important.txt` |
| `stat -c "%a %n"` | Shows **numeric permissions** of a file. | `stat -c "%a %n" file.txt` |
| `find . -perm 644` | Finds files with **specific permissions**. | `find . -perm 644` |
| `chmod 777` | Grants **full read, write, execute permissions** to everyone (use carefully). | `chmod 777 file.txt` |
| `umask 002` | Sets **default permissions** for new files to be group-writable. | `umask 002` |
| `getent passwd` | Displays **all users** on the system. | `getent passwd` |
| `getent group` | Displays **all groups** on the system. | `getent group` |
| `chown root:root file.txt` | Assigns **root as owner** of a file. | `chown root:root file.txt` |
| `chmod 644 file.txt` | Common **permission setting** for text files. | `chmod 644 file.txt` |
| `chmod 600 file.txt` | Restricts **permissions to owner only**. | `chmod 600 file.txt` |
| `chmod 400 file.txt` | Makes a file **read-only** for owner. | `chmod 400 file.txt` |

💬 **Tip:** Use `ls -l` and `stat` to verify permission changes immediately.

---
## 📦 Package Management

| Command | Description | Example |
|----------|-------------|----------|
| `apt update` | Updates the **package list/package** on Debian/Ubuntu systems — always run this before installing packages. | `sudo apt update` |
| `apt upgrade` | Upgrades **all installed packages** to the latest versions. | `sudo apt upgrade` |
| `sudo apt install bsdmainutils` | Installs the **`bsdmainutils` package** on Debian/Ubuntu-based systems. This package includes useful utilities like `cal`, `factor`, `column`, and more. | `sudo apt install bsdmainutils` |
| `apt install` | Installs a **new package** on the system from repositories.| `sudo apt install git` |
| `apt remove` | Removes an installed **package** but keeps configuration files. | `sudo apt remove nano` |
| `apt purge` | Removes a package **along with its configuration files**. | `sudo apt purge nano` |
| `apt search` | Searches the **package repository** for a package. | `apt search python3` |
| `apt show` | Displays **detailed information** about a package. | `apt show git` |
| `dpkg -i` | Installs a **.deb package** manually. | `sudo dpkg -i package.deb` |
| `dpkg -r` | Removes a **package** installed via dpkg. | `sudo dpkg -r package` |
| `yum install` | Installs a package on **RHEL/CentOS** systems. | `sudo yum install wget` |
| `yum remove` | Removes a package on **RHEL/CentOS** systems. | `sudo yum remove wget` |
| `dnf install` | Installs a package on **modern Fedora** systems. | `sudo dnf install vim` |
| `dnf remove` | Removes a package on **Fedora** systems. | `sudo dnf remove vim` |
| `dnf update` | Updates all packages on Fedora or newer RHEL systems. | `sudo dnf update` |
| `snap install` | Installs a **Snap package**. | `sudo snap install vlc` |
| `snap install` | Installs software using **Snap package manager**. | `sudo snap install code` |
| `snap remove` | Removes a Snap package. | `sudo snap remove vlc` |
| `flatpak install` | Installs a **Flatpak package**. | `flatpak install flathub org.gimp.GIMP` |
| `flatpak remove` | Removes a Flatpak package. | `flatpak remove org.gimp.GIMP` |
| `apt autoremove` | Removes **unused dependencies** automatically. | `sudo apt autoremove` |
| `apt list --installed` | Lists all **installed packages** on the system. | `apt list --installed` |
| `rpm -qa` | Lists all **installed RPM packages**. | `rpm -qa` |

💬 **Tip:** `apt list --installed` shows all packages currently installed on your system.
---

## 🗃️ Archiving & Compression

| Command | Description | Example |
|----------|-------------|----------|
| `tar -cvf` | Creates a **tar archive** of files/folders. | `tar -cvf archive.tar folder/` |
| `tar -xvf` | Extracts a **tar archive**. | `tar -xvf archive.tar` |
| `tar -czvf` | Creates a **compressed tar.gz archive**. | `tar -czvf archive.tar.gz folder/` |
| `tar -xzvf` | Extracts a **tar.gz archive**. | `tar -xzvf archive.tar.gz` |
| `zip` | Creates a **zip archive**. | `zip archive.zip file1 file2` |
| `unzip` | Extracts a **zip archive**. | `unzip archive.zip` |
| `gzip` | Compresses a **single file**. | `gzip file.txt` |
| `gunzip` | Decompresses a **.gz file**. | `gunzip file.txt.gz` |
| `bzip2` | Compresses a file using **bzip2 algorithm**. | `bzip2 file.txt` |
| `bunzip2` | Decompresses a **.bz2 file**. | `bunzip2 file.txt.bz2` |
| `xz` | Compresses files using **xz compression**. | `xz file.txt` |
| `unxz` | Decompresses a **.xz file**. | `unxz file.txt.xz` |
| `tar -cJvf` | Creates a **tar.xz archive**. | `tar -cJvf archive.tar.xz folder/` |
| `tar -xJvf` | Extracts a **tar.xz archive**. | `tar -xJvf archive.tar.xz` |
| `7z a` | Creates a **7z archive**. | `7z a archive.7z folder/` |
| `7z x` | Extracts a **7z archive**. | `7z x archive.7z` |
| `split -b 10M` | Splits a file into **10MB chunks**. | `split -b 10M bigfile.tar` |
| `cat file* > mergedfile` | Merges **split files** back together. | `cat x* > bigfile.tar` |
| `tar --delete` | Deletes a file from a **tar archive**. | `tar --delete -f archive.tar file.txt` |
| `tar -tvf` | Lists **contents of a tar archive**. | `tar -tvf archive.tar` |

---

## 💾 Disk Management

| Command | Description | Example |
|----------|-------------|----------|
| `df -h` | Shows **disk usage** of all mounted filesystems. | `df -h` |
| `du -sh` | Shows **size of files/folders** in human-readable format. | `du -sh folder/` |
| `lsblk` | Lists all **block devices** like HDDs and USB drives. | `lsblk` |
| `fdisk -l` | Displays **disk partitions and info** (requires root). | `sudo fdisk -l` |
| `parted -l` | Shows **disk partition layout**. | `sudo parted -l` |
| `mount` | Mounts a **filesystem** to a directory. | `sudo mount /dev/sdb1 /mnt` |
| `umount` | Unmounts a **mounted filesystem**. | `sudo umount /mnt` |
| `blkid` | Shows **UUIDs and filesystem types** of partitions. | `blkid` |
| `mkfs.ext4` | Formats a partition as **ext4 filesystem**. | `sudo mkfs.ext4 /dev/sdb1` |
| `fsck` | Checks and **repairs filesystem errors**. | `sudo fsck /dev/sdb1` |
| `df -i` | Displays **inode usage** on mounted filesystems. | `df -i` |
| `ls -l /dev/disk/by-uuid/` | Lists **disk UUIDs**. | `ls -l /dev/disk/by-uuid/` |
| `tune2fs -l` | Displays **ext filesystem info**. | `sudo tune2fs -l /dev/sdb1` |
| `resize2fs` | Resizes an **ext2/3/4 filesystem**. | `sudo resize2fs /dev/sdb1` |
| `mount -o remount,rw` | Remounts a **filesystem as read-write**. | `sudo mount -o remount,rw /` |
| `df -Th` | Shows **filesystem type** and disk usage. | `df -Th` |
| `ls -lh /mnt` | Displays **sizes of files** in human-readable format. | `ls -lh /mnt` |
| `stat /dev/sda1` | Shows **metadata about a disk partition**. | `stat /dev/sda1` |
| `wipefs` | Removes **filesystem signatures** from a device. | `sudo wipefs /dev/sdb1` |
| `hdparm -I` | Shows **hardware parameters** of a drive. | `sudo hdparm -I /dev/sda` |
| `df -hT` | Displays **disk usage with filesystem types**. | `df -hT` |

---
## 💾 Disk Usage with `du`

| Command | Description | Example |
|---------|-------------|---------|
| `du` | Displays the **disk usage** of files and directories (in blocks by default). | `du /home/user` |
| `du -h` | Shows disk usage in a **human-readable format** (KB, MB, GB). | `du -h /home/user/Documents` |
| `du -s` | Displays only the **total size** of the specified directory. | `du -s /home/user/Documents` |
| `du -sh` | Combines both options to show a **summarized, human-readable total size**. | `du -sh /home/user/Documents` |
| `du -sh *` | Shows a **human-readable summary for each item** in the current directory (useful to see sizes of files/folders at once). | `du -sh *` |
| `du -a` | Shows the **size of all files and directories**, not just folders. | `du -a /home/user/Documents` |
| `du -h --max-depth=1` | Shows the size of directories **one level deep** (useful for folder overviews). | `du -h --max-depth=1 /home/user` |
| `du -c` | Displays the **total disk usage** of all listed files and directories. | `du -ch /home/user/*` |
| `du -k` | Displays sizes in **kilobytes (KB)**. | `du -k /home/user/Documents` |
| `du -m` | Displays sizes in **megabytes (MB)**. | `du -m /home/user/Documents` |
| `du -h \| sort -hr \| head -n 10` | Lists the **top 10 largest directories**. | `du -h /home/user | sort -hr | head -n 10` |

💡 **Tip:** `du -sh *` is great for a quick glance at what's taking space in the current folder — pair it with `sort -hr` to list largest-first:
```bash
   du -sh * | sort -hr
```
---

## 🖥️ System Monitoring & Logs

| Command | Description | Example |
|----------|-------------|----------|
| `dmesg` | Shows **kernel and boot messages**. | `dmesg | less` |
| `journalctl` | Displays **system logs** on systemd systems. | `journalctl -xe` |
| `tail -f /var/log/syslog` | Continuously monitors a **log file**. | `tail -f /var/log/syslog` |
| `uptime` | Shows how long the system has been running and load averages. | `uptime` |
| `free -h` | Displays **RAM and swap usage** in human-readable format. | `free -h` |
| `vmstat 2` | Shows **virtual memory and CPU statistics** every 2 seconds. | `vmstat 2` |
| `iostat` | Displays **CPU and disk I/O stats**. | `iostat` |
| `sar -u 1 5` | Monitors **CPU usage** 1 second intervals, 5 times. | `sar -u 1 5` |
| `iotop` | Monitors **disk I/O by process** (requires root). | `sudo iotop` |
| `watch` | Runs a command **periodically** and shows live output. | `watch -n 2 df -h` |
| `ps aux` | Shows all **running processes** with details. | `ps aux` |
| `top` | Displays **real-time process info**. | `top` |
| `htop` | Interactive process monitor with **CPU/memory bars**. | `htop` |
| `sar -r 1 5` | Monitors **memory usage** 1 second intervals, 5 times. | `sar -r 1 5` |
| `uptime -p` | Shows **uptime in human-readable format**. | `uptime -p` |
| `journalctl -f` | **Live view** of system logs. | `journalctl -f` |
| `tail -n 50 /var/log/syslog` | Shows **last 50 lines** of syslog. | `tail -n 50 /var/log/syslog` |
| `free -m` | Displays **memory in MB**. | `free -m` |
| `vmstat -s` | Shows **memory statistics summary**. | `vmstat -s` |
| `uptime -s` | Shows **exact system boot time**. | `uptime -s` |
| `sar -b 1 5` | Monitors **I/O statistics** every 1 second, 5 times. | `sar -b 1 5` |
| `iostat -xz 2` | Detailed CPU and **disk I/O stats every 2 seconds**. | `iostat -xz 2` |
| `pidof` | Shows **PID of a running process**. | `pidof nginx` |
| `kill` | Sends a signal to **terminate a process**. | `kill 1234` |
| `kill -9` | Forces **immediate termination** of a process. | `kill -9 1234` |
| `pkill` | Kills a process by **name**. | `pkill firefox` |
| `jobs` | Lists **background jobs** in the current shell. | `jobs` |
| `fg` | Brings a **background job to foreground**. | `fg %1` |
| `bg` | Resumes a **job in the background**. | `bg %1` |
| `nice` | Sets **priority of a process**. | `nice -n 10 ./script.sh` |
| `renice` | Changes **priority of running process**. | `renice 5 -p 1234` |

---

💬 **Tip:** Use `htop` for a **friendly real-time overview** of CPU, memory, and processes. Combine `journalctl` and `tail -f` for **log monitoring**.

---
## 📬 Contributions

Contributions are always welcome! 🚀  
If you'd like to **add new commands**, **improve explanations**, or **fix errors**, simply:  
1. **Fork** this repository  
2. **Create a branch** for your feature or fix  
3. **Submit a Pull Request (PR)**  

Your contributions help make this project better for everyone. ❤️  

---

## 🧠 How to Use  

Clone the repository to your local system:  
```bash
git clone https://github.com/IrfanTech-X/Linux_Command_Line_Mastery.git
```  

Open the `README.md` file and start exploring!  
Use `Ctrl + F` (or `Cmd + F` on Mac) to quickly search for specific commands.  

### 📊 Progress Tracker  
- ✅ **300+ Commands Completed**  
- 🕓 **Regularly Updated** — new commands coming soon!  

---

## 👨‍💻 Author  

**Irfan Ferdous Siam**  
🎓 *BSc in Computer Science & Engineering*  
*Green University of Bangladesh*  
📧 **siamtalukdar3@gmail.com**  

⭐ If you find this repository helpful, consider giving it a **star** to support the project!  

> “Mastering Linux commands isn’t about memorization — it’s about thinking like the terminal.”  


