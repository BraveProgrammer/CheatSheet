![BASH Logo](bash.jpg)

**Created By _Brave Programmer_**

# **BASH Cheat Sheet**

**Requirements:**  
&nbsp;&nbsp;&nbsp;&nbsp;1. Minimal Knowledge of linux

# Working with directories

```bash
ls             # lists all of directories in path
cd folder1     # goes to folder1 if it has permission to open folder1
rmdir folder2  # deletes folder2 if it is empty
rm -r folder3  # delete folder3 with all files was in folder3
			   # -r recursive -f force
mkdir folder4  # create new directory with folder4 name
```

# Setting permissions

## Change Access Modes

```bash
chmod [perms] file
```

+ permissions:
  + r, w, x, s, S, t (read (4), write (2), execute (1), sticky bit(s, S), delete only)
    + a (all)
      + u (user)
      + g (group)
      + o (other)

**Note:** if sticky bit is on those file will run with owner of file permission

**Note 2:** s (lowercase) is suid & user's executable bit enabled but S (uppercase) is suid enabled & executable bit disabled

**Note 3:** t makes folder everyone can delete files in temp but they can't modify thems

**Note 4:** 0 is no permission

```bash
chmod u=rwx,g=rwx,o=r index.html
chmod g-w index.html
chmod 755 # User can read, write, and execute. group members and other users can read and execute, but cannot write.
chmod +t temp
```
