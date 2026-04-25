# Day 2: Creating Temporary User  

### Task Description
 Create a user named `ravi` on `App Server 3` with an expiary date `2027-01-28` for the new developer.
### Technial Implementation
 I used the `useradd` command with the `-e` flag to set the expiary date, and `-m` flag to give new developer a home directory.

- **Command:** `sudo useradd -m -e 2027-01-28 ravi` 
- **Verification:** `sudo chage -l ravi`  

### What I Learned
  Automating account expitation ensures that temporary access is revoked exactly when a project concludes, reducing the risk of orphaned accounts.