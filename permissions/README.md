# alu-shell - Permissions

This directory contains a collection of scripts that manage user permissions and ownership, as well as file and directory operations.

## Scripts

### 0-iam_betty
**Task:** Switches the current user to betty using exactly 8 characters for the command.
**Usage:** `./0-iam_betty`

### 1-who_am_i
**Task:** Prints the effective username of the current user.
**Usage:** `./1-who_am_i`

### 2-groups
**Task:** Displays all groups the current user is a member of.
**Usage:** `./2-groups`

### 3-new_owner
**Task:** Changes the owner of the file **hello** to betty.
**Usage:** `sudo ./3-new_owner`

### 4-empty
**Task:** Creates an empty file called **hello**.
**Usage:** `./4-empty`

### 5-execute
**Task:** Adds execute permission to the owner of the file **hello**.
**Usage:** `./5-execute`

### 6-multiple_permissions
**Task:** Adds execute permission to the owner and group, and read permission to others for the file **hello**.
**Usage:** `./6-multiple_permissions`

### 7-everybody
**Task:** Adds execute permission to all (owner, group, and others) for the file **hello**.
**Usage:** `./7-everybody`

### 8-James_Bond
**Task:** Sets the permissions of the file **hello** to **-------rwx** (no permissions for owner and group; full for others).
**Usage:** `./8-James_Bond`

### 9-John_Doe
**Task:** Sets the mode of the file **hello** to **-rwxr-x-wx**.
**Usage:** `./9-John_Doe`

### 10-mirror_permissions
**Task:** Sets the mode of the file **hello** to match that of the file **olleh**.
**Usage:** `./10-mirror_permissions`

### 11-directories_permissions
**Task:** Adds execute permission to all subdirectories of the current directory (using the **+** terminator) without affecting regular files.
**Usage:** `./11-directories_permissions`

### 12-directory_permissions
**Task:** Creates a directory called **my_dir** with permissions **751**.
**Usage:** `./12-directory_permissions`

### 13-change_group
**Task:** Changes the group owner of the file **hello** to **school**.
**Usage:** `sudo ./13-change_group`

### 14-change_owner_and_group
**Task:** Changes the owner and group of all files and directories in the current directory to **vincent:staff**.
**Usage:** `sudo ./14-change_owner_and_group`

### 15-symbolic_link_permissions
**Task:** Changes the owner and group of the symbolic link **_hello** to **vincent:staff**.
**Usage:** `sudo ./15-symbolic_link_permissions`

### 16-if_only
**Task:** Changes the owner of the file **hello** to **vincent** only if its current owner is **guillaume**.
**Usage:** `sudo ./16-if_only`

