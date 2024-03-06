# Gzip File Compression in Rust

This Rust program demonstrates simple file compression using the Gzip algorithm. It utilizes the `flate2` crate for compression.

## Usage

```bash
cargo run <source_file_path> <target_file_path>
```
## Dependencies

### `flate2`

The `flate2` crate is used for Gzip compression. It provides implementations of compression and decompression algorithms. You can find more information about this crate [here](https://crates.io/crates/flate2).

### `std::env`

The `std::env` module is part of the Rust standard library. It provides functions for interacting with the environment, including accessing command-line arguments. More details can be found in the [official documentation](https://doc.rust-lang.org/std/env/index.html).

### `std::fs`

The `std::fs` module is part of the Rust standard library and is used for file system operations. In this program, it's utilized for working with files, such as opening and creating files. Learn more in the [official documentation](https://doc.rust-lang.org/std/fs/index.html).

### `std::io`

The `std::io` module is a core part of the Rust standard library, offering input/output functionality. In this program, functions like `copy` and types like `BufReader` are used for efficient file handling. Explore more in the [official documentation](https://doc.rust-lang.org/std/io/index.html).

### `std::time`

The `std::time` module provides types and functions for dealing with time. In this program, the `Instant` type is used to measure the elapsed time during the compression process. Refer to the [official documentation](https://doc.rust-lang.org/std/time/index.html) for additional details.

## Example

```bash
cargo run input.txt compressed_output.gz
```

