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

### Multiple strings
```grep '208302030\|208302031\|208302032\|208302033\|208302034\|208302035\|208302036\|208302037\|208302038' *.csv```

### Order files by date (old -> new)
```ls -tr | xargs grep string```

## How to transfer files over SSH
```scp /home/myuser/folder/file.ext user@myserver.com:/myserver/tmp/name_for_file.ext```
