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
| `pwd` | Displays the full path of your **current working directory**, helping you know your exact location in the system. | `pwd` |
| `ls` | Lists all **files and directories** in the current folder. Add `-l` for detailed info or `-a` to show hidden files. | `ls -la` |
| `cd` | Changes the **current directory**. Use `cd ..` to move up one level or `cd ~` to go back to your home folder. | `cd /home/user/Documents` |
| `mkdir` | Creates a **new directory (folder)** at the specified path. | `mkdir projects` |
| `rmdir` | Removes an **empty directory**. It won’t delete folders that contain files. | `rmdir old_folder` |
| `cp` | **Copies** files or directories from one location to another. Use `-r` to copy folders recursively. | `cp file.txt /backup/` |
| `mv` | **Moves or renames** files or directories. | `mv notes.txt Documents/` |
| `rm` | **Deletes** files or directories. Use `-r` for recursive delete and `-f` to force deletion. | `rm -rf test_folder` |
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
| `cat > file` | Creates a **new file** and lets you type its content directly in the terminal. | `cat > note.txt` |
| `cat file1 file2 > newfile` | Combines multiple files into one. | `cat a.txt b.txt > combined.txt` |
| `grep` | Searches for **specific text patterns** inside files. | `grep "error" logfile.log` |
| `sort` | **Sorts lines** in a file alphabetically or numerically. | `sort names.txt` |
| `uniq` | Removes **duplicate lines** from a sorted file. | `uniq sorted.txt` |
| `wc` | Counts the **lines, words, and characters** in a file. | `wc file.txt` |
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
| `xargs` | Builds and executes commands using **input from another command**. | `find . -name "*.log" | xargs rm` |
| `cut` | Extracts **specific fields or columns** from a line of text. | `cut -d ':' -f1 /etc/passwd` |
| `paste` | **Merges lines** from multiple files side by side. | `paste file1 file2` |
| `tee` | Writes output to **both a file and the screen simultaneously**. | `ls | tee list.txt` |

💬 **Tip:** Use `ls -lh` to see file sizes in a human-readable format and `ls -lt` to sort by modification time.

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
git clone https://github.com/IrfanTech-X/Linux_Command_Line_Mastery.git
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


