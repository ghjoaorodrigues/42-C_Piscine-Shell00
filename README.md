# Shell 00

![42 Badge](https://img.shields.io/badge/42-Shell00-brightgreen)
![Shell Badge](https://img.shields.io/badge/Language-Shell-blue)
![Status Badge](https://img.shields.io/badge/Status-Completed-success)

## Project Details

For full project requirements, see the [Subject File](./subject.md).

## What I Learned

Through this foundational shell project at 42 School, I developed essential system administration and command-line skills:

- **File system navigation** - Mastered directory traversal and file manipulation commands
- **Permission management** - Learned Unix file permissions (rwx) and octal notation system
- **Shell scripting fundamentals** - Created executable scripts for automation tasks
- **Version control with Git** - Implemented Git workflows including commit history and ignore patterns
- **Text processing tools** - Utilized diff, patch, and file content manipulation utilities
- **Archive creation** - Worked with tar archives for file packaging and distribution
- **Magic file detection** - Created custom file type detection using magic numbers
- **Command-line efficiency** - Developed proficiency with complex command combinations
- **System authentication** - Worked with Kerberos tickets and authentication systems
- **Pattern matching** - Used find command with complex search criteria and actions

This project established my foundation in Unix/Linux system administration and gave me confidence working entirely through the command line interface.

## About the Project

Shell 00 is the introductory shell scripting module of the 42 C Piscine, designed to familiarize students with essential Unix/Linux command-line operations. It covers fundamental concepts including:

- File and directory operations
- Permission and attribute management
- Version control basics
- Text processing and manipulation
- System administration tasks
- Shell scripting automation

## Implementation Details

The project consists of 10 exercises that progressively build shell scripting expertise:

### File Creation and Permissions

Basic file operations and understanding Unix permission systems:

| Exercise | Focus Area | Key Skills |
|----------|------------|------------|
| ex00 - Z | File creation | Basic file output with cat |
| ex01 - testShell00 | Permission setting | chmod, file attributes |
| ex02 - Oh yeah, mooore... | Complex permissions | Advanced chmod, links, directories |

### System Administration

Working with system tools and authentication:

| Exercise | Focus Area | Key Skills |
|----------|------------|------------|
| ex03 - Connect me! | Authentication | Kerberos tickets, klist command |
| ex04 - midLS | Directory listing | ls command options, sorting, formatting |
| ex08 - clean | File management | find command, file deletion |

### Version Control

Essential Git operations and repository management:

| Exercise | Focus Area | Key Skills |
|----------|------------|------------|
| ex05 - GiT commit | Commit history | git log, commit ID extraction |
| ex06 - gitignore | Repository management | git status, ignored files |

### Text Processing

Advanced file manipulation and processing:

| Exercise | Focus Area | Key Skills |
|----------|------------|------------|
| ex07 - diff | File comparison | diff command, patch creation |
| ex09 - ft_magic | File detection | magic file creation, file command |

## Usage

Each exercise directory contains the required files:

```bash
# Navigate to exercise directory
cd ex00/

# Execute or test the solution
cat z  # For file-based exercises
bash script_name.sh  # For shell scripts
```

## Key Solutions Overview

### File Permissions Mastery
- **Binary to Octal**: Converted permission strings to numeric values
- **Symbolic Links**: Created and managed soft links between files
- **Directory Permissions**: Set proper read/write/execute permissions for directories

### Shell Scripting Automation
```bash
# Example: Git commit history (ex05)
git log --format="%H" -5

# Example: Clean temporary files (ex08)
find . \( -name "*~" -o -name "#*#" \) -print -delete
```

### System Integration
- **Kerberos Authentication**: Retrieved and displayed authentication tickets
- **File Type Detection**: Created magic signatures for custom file identification
- **Archive Management**: Packaged files using tar with specific parameters

## Technical Challenges Overcome

- **Exact Output Matching** - Ensuring commands produce precisely the required output format
- **Permission Calculation** - Converting between symbolic and octal permission representations
- **Git Command Mastery** - Learning advanced git log formatting and filtering options
- **Find Command Complexity** - Constructing complex search patterns with multiple criteria
- **Shell Compatibility** - Ensuring scripts work with /bin/sh rather than bash-specific features
- **Timestamp Handling** - Understanding how file modification times affect directory listings
- **Magic File Syntax** - Learning the specific format required for file type detection

---

*This project was completed as part of the 42 School C Piscine, demonstrating my proficiency in Unix/Linux system administration, shell scripting, and command-line tools.*

---

## License

This project is licensed under the [MIT License](./LICENSE).
