# 🐧 Linux Command Line Mastery

Welcome to **Linux Command Line Mastery** — your all-in-one guide to learning, understanding, and mastering the Linux terminal.  
This repository contains **300 essential Linux commands**, organized by category with simple explanations and examples.  

---

## 📖 About This Repository
The Linux command line is powerful — mastering it opens doors to automation, development, and system administration.  
This project helps students, developers, and enthusiasts strengthen their Linux skills through hands-on command examples.

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

## 🧭 Navigation & File Management

| Command | Description | Example |
|----------|-------------|----------|
| `pwd` | Displays the full path of your **current working directory**, so you always know where you are in the system. | `pwd` |
| `ls` | Lists all **files and directories** in the current folder. Add `-l` for detailed info or `-a` to include hidden files. | `ls -la` |
| `cd` | Changes the **current directory**. You can move to another folder, use `cd ..` to go back, or `cd ~` to return to your home directory. | `cd /home/user/Documents` |
| `mkdir` | Creates a **new directory (folder)** at the specified path. | `mkdir new_project` |
| `rmdir` | Removes an **empty directory**. If the folder has files, it won’t delete it. | `rmdir old_folder` |
| `cp` | **Copies** files or directories from one location to another. Use `-r` for copying entire directories. | `cp file.txt /backup/` |
| `mv` | **Moves or renames** files and directories. | `mv report.txt /Documents/` |
| `rm` | **Removes (deletes)** files or directories. Be careful — it’s permanent! Use `-r` to delete folders. | `rm -rf test_folder` |
| `cat` | **Displays the content** of a file directly in the terminal. Useful for quick checks. | `cat notes.txt` |
| `find` | **Searches for files** or directories within a location using patterns or filenames. | `find /home -name "example.txt"` |

💬 **Tip:** To quickly check what’s inside your folder, use `ls -lh` — it shows file sizes in a human-readable format.

---

## ⚙️ System Information

| Command | Description | Example |
|----------|-------------|----------|
| `uname -a` | Shows **detailed system and kernel information**, including OS name, version, and architecture. | `uname -a` |
| `hostname` | Displays the **system’s hostname** (the name your machine is identified by on a network). | `hostname` |
| `uptime` | Tells you **how long your system has been running** and the average CPU load. | `uptime` |
| `top` | Displays a **live view of all running processes**, their resource usage, and system load. | `top` |
| `htop` | An improved, colorful version of `top` with interactive process control. | `htop` |
| `df -h` | Shows **disk space usage** for all mounted filesystems in human-readable format. | `df -h` |
| `free -m` | Displays **memory usage** (RAM and swap) in megabytes. | `free -m` |
| `who` | Lists all **currently logged-in users**. | `who` |
| `date` | Prints the **current date and time**. | `date` |
| `cal` | Displays a **monthly calendar** right in the terminal. | `cal` |

💬 **Tip:** Use `watch -n 1 free -m` to continuously monitor memory usage in real time.

---

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

## 📦 Package Management

| Command | Description | Example |
|----------|-------------|----------|
| `apt update` | Updates the **package list** on Debian/Ubuntu systems — always run this before installing packages. | `sudo apt update` |
| `apt upgrade` | Upgrades all installed packages to the latest version. | `sudo apt upgrade` |
| `apt install` | Installs a **new package** from repositories. | `sudo apt install git` |
| `apt remove` | Removes an installed package but keeps configuration files. | `sudo apt remove nano` |
| `apt purge` | Removes a package along with its config files. | `sudo apt purge nano` |
| `yum install` | Installs a package on RHEL/CentOS systems. | `sudo yum install wget` |
| `dnf update` | Updates all packages on Fedora or newer RHEL systems. | `sudo dnf update` |
| `snap install` | Installs software using **Snap package manager**. | `sudo snap install code` |

💬 **Tip:** `apt list --installed` shows all packages currently installed on your system.

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

## 🧠 How to Use

Clone the repository to your system:
```bash
git clone https://github.com/<your-username>/Linux_Command_Line_Mastery.git
```
Then open README.md and start exploring!
You can press Ctrl + F (or Cmd + F on Mac) to search for any specific command instantly.

📊 Progress Tracker
✅ 80 / 300 Commands Completed
🕓 Updating frequently — new commands coming soon!

---

### 🧑‍💻 Author

Irfan Ferdous Siam
🎓 BSc in CSE, Green University of Bangladesh
📧 siamtalukdar3@gmail.com

⭐ Star this repository if you find it useful and want to support the project!

“Mastering Linux commands isn’t about memorization — it’s about thinking like the terminal.”


