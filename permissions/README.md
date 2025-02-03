# alu-shell - Permissions

This directory contains the following scripts:

0-iam_betty: Switches the current user to betty (using exactly 8 characters for the command).
1-who_am_i: Prints the effective username of the current user.
2-groups: Prints all groups the current user is part of.
3-new_owner: Changes the owner of the file hello to betty.
4-empty: Creates an empty file called hello.
5-execute: Adds execute permission to the owner of hello.
6-multiple_permissions: Adds execute permission to the owner and group, and read permission to others for hello.
7-everybody: Adds execute permission for all (owner, group, others) to hello.
8-James_Bond: Sets hello's permissions to -------rwx (no permissions for owner and group; full for others).
9-John_Doe: Sets the mode of hello to -rwxr-x-wx.
10-mirror_permissions: Sets the mode of hello to match that of olleh.
11-directories_permissions: Adds execute permission to all subdirectories of the current directory (using the + terminator).
12-directory_permissions: Creates a directory called my_dir with permissions 751.
13-change_group: Changes the group owner of hello to school.
14-change_owner_and_group: Changes the owner and group of all items in the working directory to vincent:staff.
15-symbolic_link_permissions: Changes the owner and group of the symbolic link _hello to vincent:staff.
16-if_only: Changes the owner of hello to vincent only if its current owner is guillaume.

