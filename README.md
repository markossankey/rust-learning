# What is this?

This is a collection of projects that I am working on to learn rust

## **Notes**

### [Section 1.](https://doc.rust-lang.org/book/ch01-03-hello-cargo.html)
*hello-world and hello_cargo*

- cargo is somewhat of a package manager / build tool (similiar to npm for node)
- run `cargo build` to build the project in a `target/*` directory, also generates a Cargo.lock file which is a form a version control for the build and its dependancies (similar to package-lock.json)
- run `cargo run` to build and run the rust files
- run `cargo check` to make sure the code compiles
- run `cargo build --release` to create an optimized build -- takes longer to generate, but produces a faster executable

### [Section 2.](https://doc.rust-lang.org/book/ch02-00-guessing-game-tutorial.html)
*guessing_game*

- To add dependencies, write them in the Cargo.toml file, then run `cargo build` to add them to the build (target/) folder
- cargo uses Semver to determine what version of a dependancy should be used.  The exact version that is used in the build command is add to the Cargo.lock file
- rust-lang.org recommends including Cargo.lock in your version control (don't add it to .gitignore)
- running `cargo update` will update the Cargo.lock file and the local package to the newest **Minor** version (i.e. if you have 0.8.5 in your Cargo.toml, it will never use anything greater than 0.8.n)
- `cargo doc --open` command will build docuementation provided by your dependencies