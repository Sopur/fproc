![alt text](https://raw.githubusercontent.com/BlueCannonBall/fproc/main/fproc.png)

# `fproc`
A process manager written in C++ and Rust.

## Motivation
After setting up cpu/memory limits for all the processes running on my server, I was astonished to find that the memory usage was still over 120 mb. After doing some probing, I found that `pm2`, a process manager, was using more cpu/memory than all my services combined!

## Usage
```
$ fproc help
fproc

USAGE:
    fproc [SUBCOMMAND]

FLAGS:
    -h, --help       Prints help information
    -V, --version    Prints version information

SUBCOMMANDS:
    delete     Delete a process
    help       Prints this message or the help of the given subcommand(s)
    list       List all managed processes.
    restart    (Re)start a process
    run        Run a process
    stop       Stop a process
```

## Building & Installing
```
$ make
# make install
```
*Note that `#` denotes a root shell, while `$` denotes a regular shell.*
