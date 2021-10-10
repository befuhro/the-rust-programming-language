# Hello world
## The main function
The main function is always the first function that is executed in Rust, it is like an entrypoint of our program.


## Compiling and executing Rust code
The file extension for Rust code should be .rs

In order to execute, we must first compile and the run the executable file created from it.
```bash
$ rustc main.rs
$ ./main
Hello, world!
``` 
Rust being a *ahead-of-time compiled* language, we can give the executable to other people and they will able to execute it without having Rust installed on their machine. 

## Println! macro
:bulb: By placing a ! at the end of our function, we are calling a macro instead of a function.
This macro does not always behave the same as the function.