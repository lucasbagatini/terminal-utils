# terminal-utils

## How to find something inside files

### Search all files in current directory
```grep string *```

### Search all files in current directory with given pattern
```grep string *.txt```

### Matching line and 1 after 
```grep -A 1 "string" *.txt```

### Matching files
```grep -l string *```

### Order files by date (old -> new)
```ls -tr | xargs grep string```

## How to transfer files over SSH
```scp /home/myuser/folder/file.ext user@myserver.com:/myserver/tmp/name_for_file.ext```
