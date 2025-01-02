# Linux Guide
> February 9th, 2023
----------------------------------------------------------------

## Viewing and Creating Files
The list command is the most basic command for viewing a file's name and metadata.

```bash
ls [OPTION] [FILE]
```

Pwd:  Prints current working directory

```bash
$ pwd
/home/John
```

Touch: Create empty files

```bash
touch test.txt
```

Mkdir: Used to create directories

```bash
mkdir new-directory
```

## Copying and Moving Files

Cp: Used to copy files

```bash
cp file1.txt /home/John/Articles/
```

Mv: Used to move files; It can also be used to rename directories or files

```bash
mv file1.txt /home/John/Articles
```

## Removing Files

Rm: Used to remove files

```bash
rm file1.txt
```

Rmdir: Used to remove directories

```bash
rmdir Articles
```

## Constructing a Soft Link

A soft link provides a pointer to a file that may reside on another filesystem which do not share the same inode numbers because they don't point to the same data. We use the ln -s/--symbolic option.

```bash
touch OriginalSFile.txt

ln -s OriginalSFile.txt SoftLinkFile.txt

ls -i
2101456 OriginalSFile.txt 2101468 SoftLinkFile.txt
```

