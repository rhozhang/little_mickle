# reove files or directory

tag: shell

>    Many a little makes a mickle

## remove files

remove all files (excluding hidden files, excluding folders) in current working directory

```bash
rm *
```

remove all hidden files (excluding folders)  in current working directory

```bash
find -maxdepth 1 -type f -name '.*' --delete
```

## remove folders

remove all files and folders (including files there), but excluding hidden files or hidden directory

```bash
rm -r *
```

here, option "-r" means "recursive", 

with option "-ri" (-r -i), prompt before every removal (-i, interactive)

list all hidden files

```bash
find -type f -name ".*"
```

delete all hidden files

```bash
find -type f -name ".*" --delete
```

list all hidden directories

```bash
find -type d -name ".*"
```

delete all hidden **empty** directories

```bash
find -type d -name ".*" -delete
```

Q: how to delete nonempty hidden directory

A: delete all files in the directory, then remove the directory, or

```bash
rm -rf .*
```

here, -f means "force"

But in this way, the warnings below prompt:

>    rm: refusing to remove '.' or '..' directory: skipping '.'
>    rm: refusing to remove '.' or '..' directory: skipping '..'

Here, "." means current folder, ".." means parent folder



