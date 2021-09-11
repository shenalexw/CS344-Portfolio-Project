# SmallShell 💾 

## Table of Contents
- [Abstract](#Abstract)
- [How To Use](#how-to-use)
- [References](#references)
- [Author(s)](#author-info)


## Abstract
CS344 Operating Systems I Portfolio Project

Replicate the funcitonality of shell in C with a subset of features known as bash.

## How To Use

### Installation
#### C Program
```
	chmod +x compile.sh
	./compile.sh
```
#### Test script
```
	chmod +x p3testscript
	./p3testscript
```
### Format Input
```
    : command [arg1 arg2 ...] [< input_file] [> output_file] [&]
```
- Command will be able to replicate most shell commands.
- Arguments may be placed into the front of the command
- Redirections of input/output are possible for single file only.
- & toggles foreground use of programs only.
    
### exit
```
    : exit
```
- Terminates all background processes and returns to the main terminal of the directory.

### cd
```
    : cd [desired directory path]
```
- Without an argument, the program will return the user to the home directory
- Go to a path through only the first argument after cd.

### status:
```
    : status
```
- Will print the status of the last process if it was terminated normally or through a signal.

### Redirection:
```
	: < input.txt > output.txt
```
- Files may be redirected following the format input above.

### ^c or ctrl+c:
```
	: ^c
```
- Terminates a foreground process and display the signal it was terminated with.
- This will not affect background processes.

### ^z or ctrl+z:
```
	: ^z
```
- Toggles between background processes being allowed or foreground processes only.

## References

- [C library function - fgets()](https://www.tutorialspoint.com/c_standard_library/c_function_fgets.htm)
- [Signal Handlers](https://linuxhint.com/signal_handlers_c_programming_language/)

## Author Info
#### Alexander Shen - Developer
- [LinkedIn](https://www.linkedin.com/in/shenalexw/)
- [Portfolio Website](https://shenalexw.github.io/)
