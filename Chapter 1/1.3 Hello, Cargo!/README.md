# Cargo
Cargo is the build system and package manager for Rust. It comes installed with Rust.

It handles tasks such as building code, downloading project's librairies and building them.

## Creating a project using Cargo
By entering the following command, it will create a directory of the same name and with a *Cargo.toml* file and a *src* directory with a *main.rs* file inside it.
```bash
$ cargo new <name_of_your_project>
```

## Cargo.toml file
This is the configuartion file of our project.

Under the [package] section, there is the name of our project, its version number and the version of the compiler that must be used to compile it.

Under the [dependencies] section, there is the dependencies used in our project.

## Source files
Source files must be placed inside the *src* directory.

## Building a project
### Debug mode
By running the following command, you will create an two executables of your program which will be *target/debug/<name_of_your_project>*. By default Cargo will build your project in debug mode.
```bash
$ cargo build
```

### Release mode
When project is built in debug mode, it will not be optimized but it will take less time to compile. Therefore it is recommended to built an optimized executable for the end user. You can do it by running the following command
```bash
$ cargo build --release
```
The executable will created will be *target/release/<name_of_your_project>*

## Running a project
By running the following command, you will build the run your project.
```bash
$ cargo run
```
:bulb: If you have already built your project and did not modify it, Cargo will only run it.

## Checking that project can compiles
As compilation can be time consuming, it can be usefull to just check that our code can compile without actually compile it. It can be done with the following command
```bash
$ cargo check
```

## Cargo.lock file
This file keeps track of the exact version of our project's dependencies. It is created and modified by Cargo and should not be edited manually.

## More information
More information can be found in the official's Cargo [documentation](https://doc.rust-lang.org/cargo/)
