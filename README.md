# Minishell

Minishell is a Unix-like shell written in C, developed as part of the 42 School curriculum. It aims to interpret and execute user commands, mimicking the behavior of the Bash shell with support for features like input/output redirection, piping, signal handling, and several built-in commands.

## Features

- **Input/Output Redirection**: Redirect output to files or input from files.
- **Piping**: Use pipes (`|`) to chain multiple commands.
- **Signal Handling**: Gracefully handle signals like `SIGINT` and `SIGQUIT`.
- **Built-in Commands**: Includes basic commands such as `cd`, `echo`, `env`, and more.

## Built-in Commands

- `cd`: Change the current directory.
- `echo`: Display a line of text.
- `env`: Show environment variables.
- `exit`: Exit the shell.
- `pwd`: Print the current working directory.
- `export`: Set environment variables.
- `unset`: Remove environment variables.

## Compilation & Usage

To compile the shell:

```bash
make
```

To run the shell:

```bash
./minishell
```

### Example Usage

```bash
$ pwd
/home/user
$ cd ..
$ echo "Hello, World!"
Hello, World!
$ ls | grep minishell > output.txt
```

## Project Structure

- **src/**: Contains the source code files.
- **libft/**: Custom C library used in the project.
- **Makefile**: Used to compile the project.

## Requirements

- **C Compiler**: Ensure you have GCC or Clang installed.
- **Make**: The project uses a Makefile for compilation.

## Learning Objectives

This project was built to strengthen knowledge in:

- System calls (e.g., `fork`, `execve`, `pipe`, `dup2`, `signal`).
- Process management and inter-process communication.
- Low-level C programming and Unix system internals.

---
