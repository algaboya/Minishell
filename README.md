# Minishell 🐚

**Minishell** is a C project from the 42 curriculum that involves creating a **mini Unix shell**. The goal is to implement a command-line interpreter that can execute commands, handle built-ins, manage pipes and redirections, and support environment variables, mimicking the behavior of a real shell like `bash`.  

---

## 📚 Table of Contents
- [Extended Description](#extended-description)  
- [Installation & Make](#installation--make)  
- [Usage](#usage)  
- [Features](#features)  
- [License](#license)  

---

## 📝 Extended Description

The **Minishell** project teaches essential concepts of shell programming and systems programming in C:  

- **Command parsing** – reading input from the user and parsing commands and arguments.  
- **Built-in commands** – implementing shell built-ins like `cd`, `echo`, `exit`, `pwd`, `export`, and `unset`.  
- **Pipes and redirections** – managing `|`, `>`, `<`, `>>` for communication between commands and file redirection.  
- **Environment variables** – handling `PATH`, user-defined variables, and variable expansion with `$`.  
- **Signal handling** – managing signals like `Ctrl+C` and `Ctrl+D` to gracefully handle interruptions.  
- **Memory management** – safely allocating and freeing memory to prevent leaks.  

By completing this project, you gain experience in **Unix system calls, process management, and building modular C programs**, which are fundamental skills for any systems programmer.  

---

## 🛠Installation & Make

Clone the repository and compile the project:

```bash
git clone https://github.com/algaoya/Minishell.git
cd minishell
make
```
## ⚙️Usage
```bash
# Start the shell
./minishell
```
Here are some command examples.

```bash
minisHell: echo "Hello, Minishell!"
Hello, Minishell!

minisHell: ls -l | grep ".c"
main.c
utils.c
minishell

minisHell: cd ..
minisHell: pwd
/home/user/42_projects

minisHell: export MY_VAR=42
minisHell: echo $MY_VAR
42

minisHell: exit
```
The shell supports interactive commands, pipes, redirections, and environment variable expansion.


---

## 🔧Features

```text
Built-in commands:
  - echo
  - cd
  - pwd
  - export
  - unset
  - env
  - exit

Command execution:
  - Execute binaries from PATH
  - Pipes (|) between commands
  - Input (<) and output (>, >>) redirection

Environment:
  - Handle environment variables
  - Variable expansion with $

Other:
  - Signal handling (Ctrl+C, Ctrl+D)
  - Error handling
```
## 📄License
This project is for educational purposes and follows the 42 school guidelines.

