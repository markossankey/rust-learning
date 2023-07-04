# Hello Cargo

[link to steps](https://doc.rust-lang.org/book/ch01-03-hello-cargo.html)

## Notes from tutorial
- cargo is somewhat of a package manager / build tool (similiar to npm for node)
- run `cargo build` to build the project in a `target/*` directory, also generates a Cargo.lock file which is a form a version control for the build and its dependancies (similar to package-lock.json)
- run `cargo run` to build and run the rust files
- run `cargo check` to make sure the code compiles
- run `cargo build --release` to create an optimized build -- takes longer to generate, but produces a faster executable
