## File System

Determine what device a directory is located on
```sh
findmnt -n -o SOURCE --target /path/to/FILE
```

Show the largest files in the filesystem
```sh
find / -xdev -type f -size +100M
```
OR
```sh
$ sudo du -a /dir/ | sort -n -r | head -n 20
```
OR
```sh
$ sudo du -a / 2>/dev/null | sort -n -r | head -n 20
```
