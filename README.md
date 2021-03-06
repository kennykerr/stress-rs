This is an informal stress test for the Rust language and toolchain using [Rust/WinRT](https://github.com/microsoft/winrt-rs). It highlights how much slower the Rust compiler is compared with modern C++ compilers. Hopefully, this can help folks working on the Rust compiler and rust-analyzer frontend.

This takes an enormous amount of time to compile. It is unfortunate that Rust seems to only support compiling a crate on a single thread.

The bindings crate produces around 160MB of Rust source code - about 3.3 million lines of code. It took 57 minutes to compile the bindings crate. Even on a single thread, this is much slower than your average C++ compiler. The comparable C++ code from [C++/WinRT](https://github.com/microsoft/cppwinrt) takes about 90 seconds to compile.
