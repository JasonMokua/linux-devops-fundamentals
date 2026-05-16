# Linux File & Directory Commands

This guide covers essential Linux commands used for creating, managing, searching, and editing files and directories.

These commands are commonly used in Linux system administration, development, and everyday terminal workflows.

---

# File & Directory Management

## 1. `touch`

Creates a new empty file.

```bash
touch filename.txt
```

Example:

```bash
touch notes.txt
```

---

## 2. `mkdir`

Creates a new directory (folder).

```bash
mkdir directory_name
```

Example:

```bash
mkdir projects
```

---

## 3. `rmdir`

Removes an empty directory.

```bash
rmdir directory_name
```

Example:

```bash
rmdir old_folder
```

---

## 4. `cp`

Copies files or directories.

```bash
cp source destination
```

Example:

```bash
cp file.txt backup.txt
```

Copy a directory recursively:

```bash
cp -r myfolder backup_folder
```

---

## 5. `mv`

Moves or renames files and directories.

```bash
mv source destination
```

Rename a file:

```bash
mv old.txt new.txt
```

Move a file to another directory:

```bash
mv file.txt /home/user/Documents
```

---

## 6. `rm`

Removes files or directories.

```bash
rm filename
```

Example:

```bash
rm notes.txt
```

Remove a directory recursively:

```bash
rm -r myfolder
```

Force remove without confirmation:

```bash
rm -rf myfolder
```

> ⚠️ Be careful when using `rm -rf` because deleted files cannot be easily recovered.

---

# File Searching & Viewing

## 7. `find`

Searches for files and directories.

```bash
find [path] [options] [expression]
```

Example:

```bash
find . -name "file.txt"
```

---

## 8. `less`

Views file contents one page at a time.

```bash
less filename
```

Example:

```bash
less log.txt
```

---

## 9. `head`

Displays the first 10 lines of a file by default.

```bash
head filename
```

Example:

```bash
head data.txt
```

Show the first 20 lines:

```bash
head -20 data.txt
```

---

## 10. `tail`

Displays the last 10 lines of a file by default.

```bash
tail filename
```

Example:

```bash
tail log.txt
```

Monitor a file in real time:

```bash
tail -f log.txt
```

---

# Text Editors

## 11. `nano`

A simple and beginner-friendly terminal text editor.

```bash
nano filename
```

Example:

```bash
nano notes.txt
```

---

## 12. `vim`

A powerful and advanced terminal text editor.

```bash
vim filename
```

Example:

```bash
vim script.sh
```

---

# Text Processing Commands

## 13. `grep`

Searches for text patterns inside files.

```bash
grep "pattern" filename
```

Example:

```bash
grep "error" log.txt
```

Case-insensitive search:

```bash
grep -i "error" log.txt
```

---

## 14. `sort`

Sorts lines in a file alphabetically or numerically.

```bash
sort filename
```

Example:

```bash
sort names.txt
```

---

## 15. `uniq`

Removes duplicate adjacent lines from sorted input.

```bash
uniq filename
```

Example:

```bash
uniq names.txt
```

Commonly used with `sort`:

```bash
sort names.txt | uniq
```

---

## 16. `wc`

Counts lines, words, and characters in a file.

```bash
wc filename
```

Example:

```bash
wc notes.txt
```

Count only lines:

```bash
wc -l notes.txt
```

---

## 17. `cut`

Extracts specific columns or characters from a file.

```bash
cut [options] filename
```

Example:

```bash
cut -d "," -f1 data.csv
```

---

## 18. `awk`

A powerful text-processing tool used for pattern scanning and data extraction.

```bash
awk 'pattern {action}' filename
```

Example:

```bash
awk '{print $1}' data.txt
```

---

# Summary

These Linux commands form the foundation of file and text management in the terminal. Mastering them will improve your efficiency when working with Linux systems, shell scripting, and server administration.
