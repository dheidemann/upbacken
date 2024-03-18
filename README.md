# upbacken
Script to handle backups with a running nextcloud instance
```
Commands:
    init                Initialize nextcloud connection
    sync                Sync local folders with cloud
    add                 Add backup path: [-p <local path>] [-d <dest path>]
    rm                  Delete path
```

## install
1. I suggest you add this folder to your path
2. `upbacken init`

## usage
- Add all paths to backup via `upbacken add -p Documents/stuff -d important/stuff`
    - `-p` is optional. If not given, the current directory it is
    - `-d` is the destination path on nextcloud
- Remove paths: `upbacken rm`. A prompt shows all paths and asks to delete
- Sync with remote nextcloud: `upbacken sync`
