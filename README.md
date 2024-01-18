# Intern-Manager
A command-line tool for server administration tasks.<br>

Overview internsctl provides a convenient way to manage various server-related tasks, including:<br> 
Retrieving system information (CPU, memory)<br> 
Managing users (creating, listing)<br> 
Obtaining file details<br>

Make the script executable: <br> 
  chmod +x internsctl<br>

For using tool globally in linux terminal, move the script to /usr/local/bin with root user.<br>

For installing manual page of this tool: <br> 
sudo install -g 0 -o 0 -m 0644 internsctl.1 /usr/share/man/man1/<br>

Usage:<br>  
internsctl [options] [arguments]<br>

Commands: cpu getinfo: Get detailed CPU information.<br> 
memory getinfo: Display memory usage information.<br> 
user create : Create a new user with a home directory.<br> 
user list [--sudo-only]: List all users or only those with sudo privileges.<br> 
file getinfo [options] : Display information about a file.<br>

Options Global options:<br> 
--help: Display the help message.<br> 
--version: Print the script version.<br>

file getinfo options: <br>
--size, -s: Print the file size in bytes.<br> 
--permissions, -p: Show file access permissions.<br> 
--owner, -o: Display the file owner username.<br> 
--last-modified, -m: Print the file's last modification time.
