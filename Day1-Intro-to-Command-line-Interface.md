# Intro to Command-line Interface (CLI)

# Goals

- Understand what is terminal, shell, bash and other terms
- Study commands used to operate your OS
- When you need to manage a remote server and you don't have access to a graphical interface, you need to know some basic commands to operate your OS.
- Better understanding of what we do when executing a command
- Be confident to use the black screen

# Agenda

- What is the command-line?
- Why use it?
- What is the shell?
- What is Bash?
- Syntax
- Examples
- Tricks

# What is the command-line?

- The command-line is a text interface for your computer.
- It's a program that takes in commands, which it passes on to the computer's operating system to run.
- You can see results of the commands you run on the command-line.
- You can also use the command-line to interact with programs that have a CLI.
- The command-line is also known as the terminal, console, command prompt, shell, bash, and more.

# Why use it?

- The command-line is a powerful tool.
- It's faster to operate on the command-line than using a mouse and graphical interface.
- Some tasks can only be done on the command-line.
- It's more reliable to automate tasks on the command-line than using a mouse and graphical interface.
- It's easier to connect the command-line to other programs and scripts.
- It's easier to search for help online when using the command-line, because many people use the command-line.
- When you need to manage a remote server and you don't have access to a graphical interface, you need to know some basic commands to operate your OS.

# What is the shell?

- The shell is a program that takes in commands and passes them to the operating system to run.
- The shell is also known as the command-line interpreter, command processor, or command language interpreter.
- The shell is what interprets the commands you type into the command-line.

# What is Bash?

- Bash is an acronym for Bourne Again SHell.
- Bash is a specific type of shell, which is the most common shell on Linux and Mac.
- Bash is also the default shell on Ubuntu.

# Syntax

> _command_ | _option(s)_ | _argument(s)_

## Command

- Command is the action to be executed.
- Commands are case-sensitive.

## Options

- Options are optional.
- Options are used to modify the behavior of the command.
- Options are preceded by a dash (`-`).
- One dash (`-`) for single-letter options. Can combine with other single-letter options.
- Two dashes (`--`) for multi-letter options. Can't combine with other options.
- Options are case-sensitive.

## Arguments

- Arguments are optional.
- Arguments are used to specify the target of the command.
- Can be additional data or path to a file or directory.

# Examples

| Command   | Options | Arguments                     | Description                                                     |
| --------- | ------- | ----------------------------- | --------------------------------------------------------------- |
| `echo`    | ---     | `Hello World!`                | Print a string                                                  |
| `echo`    | ---     | `Hello World!` > `hello.txt`  | Create a new file and add content or override existing content  |
| `echo`    | ---     | `Hello World!` >> `hello.txt` | Create a new file and add content or append to existing content |
| `pwd`     | ---     | ---                           | Print current working directory                                 |
| `cd`      | ---     | ---                           | Change directory                                                |
| `cd`      | `~`     | ---                           | Change directory to home directory                              |
| `cd`      | `.`     | ---                           | Current directory                                               |
| `cd`      | `..`    | ---                           | Change directory to parent                                      |
| `ls`      | `-l`    | ---                           | List files in current directory with more information           |
| `ls`      | `-a`    | ---                           | List all files in current directory                             |
| `ls`      | `-h`    | ---                           | List files in current directory with human readable sizes       |
| `ls`      | `-R`    | ---                           | List files in current directory recursively                     |
| `ls`      | `-S`    | ---                           | List files in current directory sorted by size                  |
| `ls`      | `-t`    | ---                           | List files in current directory sorted by time                  |
| `ls`      | `-r`    | ---                           | List files in current directory in reverse order                |
| `file`    | ---     | `filepath`                    | Determine file type                                             |
| `stat`    | ---     | `filepath`                    | Display file owner, permission, size, etc                       |
| `mkdir`   | ---     | `dirname`                     | Create a directory                                              |
| `mkdir`   | `-p`    | `dirname/dirname`             | Create a directory and parent directories if needed             |
| `touch`   | ---     | `filepath`                    | Create a file                                                   |
| `cp`      | ---     | `source` `target`             | Copy a file                                                     |
| `cp`      | `-r`    | `source` `target`             | Copy a directory                                                |
| `mv`      | ---     | `source` `target`             | Move a file or directory                                        |
| `rm`      | ---     | `filepath`                    | Remove a file                                                   |
| `rm`      | `-r`    | `filepath`                    | Remove a directory                                              |
| `rm`      | `-f`    | `filepath`                    | Force to remove a file without confirmation                     |
|           | `*`     | ---                           | Wildcard, matches any character                                 |
|           | `?`     | ---                           | Wildcard, matches any single character                          |
|           | `[]`    | ---                           | Wildcard, matches any character in the brackets                 |
|           | `!`     | ---                           | Wildcard, matches any character not in the brackets             |
| `find`    | `-name` | `filename`                    | Find files by name                                              |
| `find`    | `-type` | `f`                           | Find files by type                                              |
| `find`    | `-type` | `d`                           | Find directories by type                                        |
| `find`    | `-size` | `+100M`                       | Find files by size                                              |
| `cat`     | ---     | `filepath`                    | Display the contents of a file                                  |
| `less`    | ---     | `filepath`                    | Display the contents of a file                                  |
| `head`    | ---     | `filepath`                    | Display the first 10 lines of a file                            |
| `head`    | `-n`    | `filepath`                    | Display the first n lines of a file                             |
| `tail`    | ---     | `filepath`                    | Display the last 10 lines of a file                             |
| `tail`    | `-n`    | `filepath`                    | Display the last n lines of a file                              |
| `nano`    | ---     | `filepath`                    | Edit a file                                                     |
| `vim`     | ---     | `filepath`                    | Edit a file                                                     |
| `man`     | ---     | `command`                     | Display the manual page of a command (`Q` to leave)             |
| `apropos` | ---     | `keyword`                     | Search the manual page for a keyword (`Q` to leave)             |
| `clear`   | ---     | ---                           | Clear the screen                                                |

# Tricks

| Command                        | Description          |
| ------------------------------ | -------------------- |
| `tab`                          | Auto-complete        |
| `arrow up`                     | Previous command     |
| `arrow down`                   | Next command         |
| `ctrl (option on Mac) + arrow` | Move cursor by word  |
| `ctrl+a`                       | Move cursor to start |
| `ctrl+e`                       | Move cursor to end   |
| `ctrl+u`                       | Delete to start      |
| `ctrl+k`                       | Delete to end        |

# Activity

Try to complete all the challenges.

[Command Challenge](https://cmdchallenge.com/#/hello_world)
