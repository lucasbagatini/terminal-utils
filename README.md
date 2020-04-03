# terminal-utils

## How to find something inside files

### Search all files in current directory
```grep string *```

### Matching files
```grep -l string *```

### Order files by date (old -> new)
```ls -tr | xargs grep string```
