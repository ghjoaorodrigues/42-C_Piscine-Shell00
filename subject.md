# Shell 00

## 📘 Project Overview

**Shell 00** is a foundational shell scripting project from the 42 C Piscine curriculum. Its goal is to introduce students to basic shell commands, file permissions, version control, and system administration concepts through hands-on exercises.

> **Disclaimer:**  
> This document is an unofficial summary written for educational and documentation purposes.  
> It is not affiliated with or endorsed by 42 or its partners.  
> All 42 students are responsible for adhering to the academic integrity policy.  
> You may **not** publish or share any part of the official subject PDF, evaluation scripts, or Moulinette content.

---

## Contents

- [Goals](#goals)
- [General Requirements](#general-requirements)
- [Exercise 00 - Z](#exercise-00---z)
- [Exercise 01 - testShell00](#exercise-01---testshell00)
- [Exercise 02 - Oh yeah, mooore...](#exercise-02---oh-yeah-mooore)
- [Exercise 03 - Connect me!](#exercise-03---connect-me)
- [Exercise 04 - midLS](#exercise-04---midls)
- [Exercise 05 - GiT commit](#exercise-05---git-commit)
- [Exercise 06 - gitignore](#exercise-06---gitignore)
- [Exercise 07 - diff](#exercise-07---diff)
- [Exercise 08 - clean](#exercise-08---clean)
- [Exercise 09 - Illusions, not tricks, Michael...](#exercise-09---illusions-not-tricks-michael)
- [Submission Guidelines](#submission-guidelines)

---

## Goals

- Learn basic shell commands and file system navigation.
- Understand file permissions and attributes.
- Master version control concepts with Git.
- Practice shell scripting and command-line tools.
- Develop system administration skills.

---

## General Requirements

- Exercises must be executable with `/bin/sh`.
- Follow the submission procedures for every exercise.
- Exercises are ordered by difficulty - easier ones must be completed first.
- Ensure appropriate permissions on files and directories.
- No additional files beyond those specified in the subject.
- Evaluation includes peer reviews and automated testing via **Moulinette**.
- Reference materials: Google, man pages, the Internet, forum discussions.

---

## Exercise 00 - Z

**Turn-in directory:** `ex00/`  
**Files to turn in:** `z`  
**Allowed functions:** None

Create a file called `z` that returns "Z" followed by a newline when using the `cat` command.

**Expected output:**
```bash
?> cat z
Z
?>
```

---

## Exercise 01 - testShell00

**Turn-in directory:** `ex01/`  
**Files to turn in:** `testShell00.tar`  
**Allowed functions:** None

Create a file called `testShell00` with specific permissions to match this output:

```bash
%> ls -l
total 1
-r--r-xr-x 1 XX XX 40 Jun 1 23:42 testShell00
%>
```

Once achieved, create the submission file:
```bash
tar -cf testShell00.tar testShell00
```

> Note: "XX" values and timestamp variations are acceptable.

---

## Exercise 02 - Oh yeah, mooore...

**Turn-in directory:** `ex02/`  
**Files to turn in:** `exo2.tar`  
**Allowed functions:** None

Create files and directories to match this exact `ls -l` output:

```bash
%> ls -l
total XX
drwx--xr-x 2 XX XX XX Jun 1 20:47 test0
-rwx--xr-- 1 XX XX 4 Jun 1 21:46 test1
dr-x---r-- 2 XX XX XX Jun 1 22:45 test2
-r-----r-- 2 XX XX 1 Jun 1 23:44 test3
-rw-r----x 1 XX XX 2 Jun 1 23:43 test4
-r-----r-- 2 XX XX 1 Jun 1 23:44 test5
lrwxr-xr-x 1 XX XX 5 Jun 1 22:20 test6 -> test0
%>
```

Create submission file: `tar -cf exo2.tar *`

---

## Exercise 03 - Connect me!

**Turn-in directory:** `ex03/`  
**Files to turn in:** `klist.txt`  
**Allowed functions:** None

Ensure you have a valid (non-expired) Kerberos ticket, then write a list of all your tickets into `klist.txt`.

> Note: These commands will be useful later - remember them!

---

## Exercise 04 - midLS

**Turn-in directory:** `ex04/`  
**Files to turn in:** `midLS`  
**Allowed functions:** None

Create a `midLS` file containing a command that lists all files and directories in the current directory:
- Exclude hidden files (starting with dots, including `.`)
- Separate entries with commas
- Order by creation date
- Add slash `/` after directory names
- Show only what's requested

---

## Exercise 05 - GiT commit

**Turn-in directory:** `ex05/`  
**Files to turn in:** `git_commit.sh`  
**Allowed functions:** None

Create a shell script that displays the IDs of the last 5 commits from your git repository.

**Expected output:**
```bash
%> bash git_commit.sh | cat -e
baa23b54f0adb7bf42623d6d0a6ed4587e11412a$
2f52d74b1387fa80eea844969e8dc5483b531ac1$
905f53d98656771334f53f59bb984fc29774701f$
5ddc8474f4f15b3fcb72d08fcb333e19c3a27078$
e94d0b448c03ec633f16d84d63beaef9ae7e7be8$
%>
```

---

## Exercise 06 - gitignore

**Turn-in directory:** `ex06/`  
**Files to turn in:** `git_ignore.sh`  
**Allowed functions:** None

Write a shell script that lists all existing files ignored by your Git repository.

**Example output:**
```bash
%> bash git_ignore.sh | cat -e
.DS_Store$
mywork.c~$
%>
```

---

## Exercise 07 - diff

**Turn-in directory:** `ex07/`  
**Files to turn in:** `b`  
**Allowed functions:** None

Create a file `b` such that when you run `diff a b > sw.diff`, it produces the expected patch file.

Reference the provided file `a` with Star Wars content. Use `man patch` for guidance.

---

## Exercise 08 - clean

**Turn-in directory:** `ex08/`  
**Files to turn in:** `clean`  
**Allowed functions:** None

Create a file called `clean` containing a single command that:
- Searches current directory and subdirectories
- Finds files ending with `~`
- Finds files starting and ending with `#`
- Shows and erases all found files
- Uses only one command (no `;`, `&&`, or other operators)

Reference: `man find`

---

## Exercise 09 - Illusions, not tricks, Michael...

**Turn-in directory:** `ex09/`  
**Files to turn in:** `ft_magic`  
**Allowed functions:** None

Create a magic file called `ft_magic` that detects files of "42 file type" - files containing the string "42" at the 42nd byte.

Reference: `man file`

---

## Submission Guidelines

- Submit exercises in order of difficulty.
- Ensure proper file permissions and directory structure.
- Follow exact naming conventions.
- Code will be evaluated by peers and Moulinette.
- Moulinette evaluation is strict and automated.
- Submit to the Git repository assigned by 42.

---

## Testing

Test your solutions thoroughly:
- Verify file permissions with `ls -l`
- Test commands in different environments
- Ensure scripts work with `/bin/sh`
- Check output formatting exactly matches requirements

---

## Final Note

This module introduces essential shell skills that form the foundation for system administration and development workflows at 42. Master these basics as they will be crucial throughout the curriculum.