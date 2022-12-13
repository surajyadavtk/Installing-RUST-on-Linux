# Installation of RUST on Linux(Ubuntu 22.04)
## 1. Updating Ubuntu
- Before installing RUST, first update ubuntu system to get latest version of packages.
    - `$ sudo apt update && sudo apt upgrade`
## 2. Install Rust Dependencies
- For RUST various packages need to be installed.
    - `$ sudo apt install -y curl gcc make build-essential`
## 3. Download and install RUST
- Download RUST installations scripts from *curl*.
- Here **rustup shell script** is used.
    - `$ curl https://sh.rustup.rs -sSf | sh`
- After it will prompt to various installation type(choose *default*)
## 4. Configure
- After installation, configure current shell for RUST environment.
    - `$ source ~/.profile`
    - `$ source ~/.cargo/env`
## 5. Verify
- Confirm installation by checking its version.
    - `$ rustc -V`

# Writing First RUST Program

- Create project directory to store RUST code.
    - `$ mkdir rust_demo`
- Navigate to created directory and open editor(*vi,nano*)
    - `$ cd rust_demo && nano helloworld.rs`
- Write code as below:
     ```
        fn main() {
            println!("Hello world!");
        }
    ```
- Save file(*ctrl+o*) and exit(*ctl+x*) the editor.
- Compile RUST file.
    - `$ rustc helloworld.rs`
- Execute by creating executable file.
    - `$ ./helloworld`
- Output
    ```
    Hello world!
    ```
