# stress-rs

This is an informal stress test for the Rust language and toolchain using Rust/WinRT. It highlights how much slower the Rust compiler is compared with modern C++ compilers. Hopefully, this can help folks working on the Rust compiler and rust-analyzer frontend.

This takes an enormous amount of time to compile. It is unfortunate that Rust seems to only support compiling a crate on a single thread.

The bindings crate produces around 160MB of Rust source code. It took 57 minutes to compile the bindings crate.