# Day 1: Creating a Non-Interactive User  

### Task Description Create a user named `john` on `App Server 1` with a non-interactive shell to accommodate a backup agent's requirements.  

### Technial Implementation I used the `useradd` command with the `-s` flag to specify the shell. 

- **Command:** `sudo useradd -s /sbin/nologin john` 
- **Verification:** `grep john /etc/ passwd`  

### What I Learned  A non-interactive shell (like `/sbin/nologin) prevents a user from logging into the system via SSH or a local terminal, which is a security best practice for service accounts.g