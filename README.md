# Simple Shell

Simple OS shell written in C for Unix-type systems.

Basic command line interface that allows the user to interact the with the operating system by entering commands and receiving appropriate output.

## Features

- Built in commands
- Searches for executables on PATH enviroment variable
- History (saves the last 20 commands)
- Command aliasing with cylical alias detection

## Built-in command usage

### Basic usage

- `cd` - change working directory
- `getpath` - print the system path
- `setpath` - set the system path

### History

- `history` - Print history contents (numbered list of commands in history including their parameters in ascending order from least to most recent)
- `!!` - Invoke the last command frmo history
- `!<no>` - Invoke command with number `<no>` from history (e.g. `!5` will excecute the command with number 5 from history)
- `!-<no>` - Invoke command with the number the number of current commands minus `<no>` (e.g. `!-3` if the current command number is 5 will execute the command with number 2, or `!-1` will execute again the last command)

### Alias

- `alias` - Print all set aliases (alias plus aliased command)
- `alias <name> <command>` - alias name to be the command. Command can include any number of parameters
- `unalias <name>` - remove any associated alias
