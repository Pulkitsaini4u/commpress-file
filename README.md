**Gzip File Compression in Rust**
This Rust program demonstrates a simple file compression using the Gzip algorithm. It utilizes the flate2 crate, which provides implementations of compression and decompression algorithms.

**Usage**
Ensure you have Rust installed on your system. Follow these steps to compile and run the program:

Clone the repository or create a new Rust project.
Navigate to the project directory.

Compile and run the program with Cargo using the following command:
  **cargo run <source_file_path> <target_file_path>**
  <source_file_path>: Path to the file you want to compress.
  <target_file_path>: Path to the output compressed file.

Dependencies
flate2: A crate used for Gzip compression.
std::env: Provides access to command-line arguments.
std::fs: Allows working with files.
std::io: Facilitates input/output operations and stream handling.
std::time: Used for measuring time durations.

Example
cargo run file.pdf compressed_output.gz
This command compresses the file named input.txt and saves the compressed output as compressed_output.gz.

Explanation of Code
The code is well-documented to explain each part's purpose and functionality in simple terms. Here's a brief overview:

Imports: Necessary crates and modules are imported, including flate2 for compression and various standard library modules for file handling and time measurement.

Main Function: The entry point of the program where the file compression process occurs.

Command-line Arguments: The program expects two command-line arguments: the source file path and the target file path. It checks for the correct number of arguments and displays a usage message if incorrect.

File Handling: It opens the source file for reading and creates the target file for writing the compressed data.

Compression Process: The data from the source file is copied to a Gzip encoder, which compresses the data. The compressed output is then written to the target file.

Output Information: After compression, the program displays the size of the source file before compression and the size of the compressed output. It also shows the elapsed time for the compression process.

Author
Pulkit Saini

License
This project is licensed under the MIT License - see the LICENSE.md file for details.
