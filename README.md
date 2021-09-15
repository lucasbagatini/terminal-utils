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

---

## Order files by date (old -> new)
```ls -tr | xargs grep string```

## How to transfer files over SSH
```scp /home/myuser/folder/file.ext user@myserver.com:/myserver/tmp/name_for_file.ext```

## How to append the output of a command to the end of a file
```command &>> output.txt```

## How to copy a folder from a docker container
```docker cp container_name:/path/to/container/folder /path/to/external/dir```

## How to use mysqldump inside docker container
```
docker exec -it container_name mysqldump -u root --password=123456 schema_name --fields-terminated-by ',' /
--fields-enclosed-by '"' --fields-escaped-by '\' /
--no-create-info --tab /var/lib/mysq-files/
```

## How to copy multiple times the content from one file to another 
```for i in {1..25}; do cat 02122020_log.csv >> 02122020_log_huge.csv; done```

## Stop asking for passphrase for given key
```ssh-add /Users/my_user/.ssh/id_ed25519```

## How to stop a process by port number
```kill -9 $(lsof -t -i tcp:8080)```

