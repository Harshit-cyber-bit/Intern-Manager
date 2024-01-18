# Intern-Manager
A command-line tool for server administration tasks.

Overview internsctl provides a convenient way to manage various server-related tasks, including: Retrieving system information (CPU, memory) Managing users (creating, listing) Obtaining file details

Make the script executable: Bash chmod +x internsctl

For using tool globally in linux terminal, move the script to /usr/local/bin with root user.

For installing manual page of this tool: Bash sudo install -g 0 -o 0 -m 0644 internsctl.1 /usr/share/man/man1/

Usage: Bash internsctl [options] [arguments]

Commands: cpu getinfo: Get detailed CPU information. 
memory getinfo: Display memory usage information. 
user create : Create a new user with a home directory. 
user list [--sudo-only]: List all users or only those with sudo privileges. 
file getinfo [options] : Display information about a file.

Options Global options: 
--help: Display the help message. 
--version: Print the script version.

file getinfo options: <br>
--size, -s: Print the file size in bytes. 
--permissions, -p: Show file access permissions. 
--owner, -o: Display the file owner username. 
--last-modified, -m: Print the file's last modification time.
