# My OS

## About the project
I love learning about new stuff and implementing low-level code, so in this repo I developed an OS based on [OS Phill](https://os.phil-opp.com/).

## How to run/test
You need to install `rust` on your system. Afterwards, you have to activate the `nightly` version:
```
$ rustup override set nightly
```
To test the project:
```
$ cargo test
``` 
To run the kernel, you have to install `qemu` on your system. Then:
```
$ cargo build
$ qemu-system-x86_64 -drive format=raw,file=target/x86_64-OS/debug/bootimage-my_os.bin
```

A simple `cargo run` would work as well!
