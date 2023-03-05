# About this Repo

This is the Git repo of the Docker unofficial image for rust. In the Docker images, I configured the mirror address of Rust's Crates.io source to the mirror hosted by the University of Science and Technology of China (USTC).

## Usage

For example, the Docker images can be used to build a Rust project.

```
doker run --rm --user "$(id -u)":"$(id -g)" -v "$PWD":/usr/src/myapp -w /usr/src/myapp therainisme/rust:1.67.1 cargo build --release
```