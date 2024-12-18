Live URL:   https://aminbiography.github.io/linux/

![kali-linux](https://i.pinimg.com/736x/fc/8f/66/fc8f6679f94fe93fc6fff400827f4173.jpg)


<h1>Here are some essential Linux commands that every Linux user should know.</h1>

<h2>01: Navigating the File System</h2>

<p>pwd</p> 
<p></p>Prints the current working directory.</p>

```
pwd
```

<p>cd <directory></directory></p> 
<p>Changes the current directory to <directory>. To go back to the previous directory, use cd -.</p>

```
cd /home/user
```

<p>ls</p> 
<p>Lists the files and directories in the current directory. Use ls -l for detailed information and ls -a to include hidden files.</p>

```
ls -l
```

<p>cd ~</p>
<p>Moves to the user's home directory.</p>

```
cd ~
```

<h2>02: Managing Files and Directories</h2>

<p>mkdir <directory></p>
<p>Creates a new directory.</p>

```
mkdir new_folder
```

<p>touch <file></p>
<p>Creates a new empty file or updates the timestamp of an existing file.</p>

```
touch file.txt
```

<p>cp <source> <destination></p>
<p>Copies files or directories. Use -r to copy directories recursively.</p>

```
cp file1.txt file2.txt
```

<p>mv <source> <destination></p>
<p>Moves or renames files and directories.</p>

```
mv file1.txt /home/user/docs/
```

<p>rm <file></p>
<p>Removes a file. Use -r for directories and -f to force remove without prompt.</p>

```
rm file.txt
rm -r folder
```

<h2>03: Viewing and Manipulating Files</h2>

<p>cat <file></p>
<p>Displays the contents of a file.</p>

```
cat file.txt
```

<p>less <file></p>
<p>Allows you to view the contents of a file one screen at a time.</p>

```
less file.txt
```

<p>head <file></p>
<p>Displays the first 10 lines of a file (use -n to specify a different number).</p>

```
head file.txt
```

<p>tail <file></p>
<p>Displays the last 10 lines of a file (use -n for a different number).</p>

```
tail file.txt
```

<p>grep <pattern> <file></p>
<p>Searches for a pattern inside a file.</p>

```
grep "search_text" file.txt
```

<h2>04: File Permissions</h2>

<p>chmod <permissions> <file></p>
<p>Changes the permissions of a file or directory. Use r, w, x for read, write, and execute.</p>

```
chmod 755 script.sh
```

<p>chown <user>:<group> <file></p>
<p>Changes the owner and/or group of a file or directory.</p>

```
chown user:group file.txt
```

<h2>05: Process Management</h2>

<p>ps</p>
<p>Displays the current processes running on the system.</p>

```
ps aux
```

<p>top</p>
<p>Displays system processes and resource usage in real-time.</p>

```
top
```

<p>kill <pid></p>
<p>Terminates a process by its process ID (PID).</p>

```
kill 1234
```

<p>killall <process_name></p>
<p>Terminates all processes with the given name.</p>

```
killall firefox
```

<p>bg</p>
<p>Resumes a paused job in the background.</p>

```
bg
```

<p>fg</p>
<p>Brings a background job to the foreground.</p>

```
fg
```

<h2>06: Disk Usage</h2>

<p>df</p>
<p>Displays disk space usage of file systems.</p>

```
df -h
```

<p>du</p>
<p>Shows disk usage for files and directories.</p>

```
du -sh /path/to/directory
```

<h2>07: Networking</h2>

<p>ping <host></p>
<p>Pings a host (IP or domain) to check network connectivity.</p>

```
ping google.com
```

<p>ifconfig or ip a</p>
<p>Displays network interfaces and their configurations.</p>

```
ifconfig
```

<p>netstat</p>
<p>Displays network connections, routing tables, interface statistics, and more.</p>

```
netstat -tuln
```

<h2>08: Package Management</h2>

<p>apt-get (Debian-based)</p>
<p>Used for package installation, removal, and updates (e.g., on Ubuntu).</p>

```
sudo apt-get update
sudo apt-get install <package>
```

<p>yum (Red Hat-based)</p>
<p>Used for package management in Red Hat-based distributions like CentOS.</p>

```
sudo yum install <package>
```

<p>dnf (Fedora-based)</p>
<p>A newer package manager for Fedora and CentOS.</p>

```
sudo dnf install <package>
```

<h2>09: Searching for Files</h2>

<p>find <directory> -name <filename></p>
<p>Searches for files within a directory hierarchy.</p>

```
find /home/user -name "file.txt"
```

<p>locate <filename></p>
<p>Searches for files using a prebuilt index (faster than find).</p>

```
locate file.txt
```

<h2>10: Archiving and Compression</h2>

<p>tar</p>
<p>Archives files. Use -czf to create a compressed archive and -xzf to extract.</p>

```
tar -czf archive.tar.gz folder
tar -xzf archive.tar.gz
```

<p>gzip</p>
<p>Compresses files using the gzip algorithm.</p>

```
gzip file.txt
```

<p>unzip</p>
<p>Extracts files from a .zip archive.</p>

```
unzip archive.zip
```

<h2>11: User Management</h2>

<p>useradd <username></p>
<p>Adds a new user.</p>

```
sudo useradd newuser
```

<p>passwd <username></p>
<p>Changes the password for a user.</p>

```
sudo passwd newuser
```

<p>whoami</p>
<p>Displays the current logged-in user.</p>

```
whoami
```

<h2>12: System Information</h2>

<p>uname -a</p>
<p>Displays detailed information about the system kernel.</p>

```
uname -a
```

<p>uptime</p>
<p>Shows how long the system has been running, along with the load averages.</p>

```
uptime
```

<p>free</p>
<p>Displays memory usage.</p>

```
free -h
```

<h2>13: Help and Manual Pages</h2>

<p>man <command></p>
<p>Displays the manual page for a command.</p>

```
man ls
```

<p>--help</p>
<p>Provides a brief help message for a command.</p>

```
ls --help
```

<h2>14: Environment Variables</h2>

<p>export <variable_name>=<value></p>
<p>Sets environment variables for the current session. This is useful for configuring paths and settings.</p>

```
export PATH=$PATH:/new/directory/path
```

<p>echo $<variable_name></p>
<p>Displays the value of an environment variable.</p>

```
echo $PATH
```

<h2>15: Viewing and Monitoring System Logs</h2>

<p>dmesg</p>
<p>Displays system messages and logs, often used for troubleshooting hardware and kernel-related issues.</p>

```
dmesg | less
```

<p>journalctl</p>
<p>Views logs collected by systemd (on systems using systemd). Use -xe for more detailed, real-time logs.</p>

```
journalctl -xe
```


![kali-linux](https://i.pinimg.com/736x/fc/8f/66/fc8f6679f94fe93fc6fff400827f4173.jpg)
