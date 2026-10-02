# yes-rs 🚀

![yes-rs](https://img.shields.io/badge/version-1.0.0-brightgreen.svg) ![Rust](https://img.shields.io/badge/rust-1.58.0-orange.svg) ![License](https://img.shields.io/badge/license-MIT-blue.svg)

A blazingly fast, memory-safe rewrite of the classic Unix `yes` command. Written in Rust! 🦀

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Introduction

The `yes` command is a simple yet powerful tool that outputs a string repeatedly until it is killed. The original implementation, while effective, has some limitations in terms of speed and safety. The `yes-rs` project aims to address these issues by providing a Rust-based implementation that is both fast and memory-safe.

Rust is known for its focus on safety and performance. By rewriting the `yes` command in Rust, we leverage these strengths to create a tool that not only performs well but also adheres to modern programming standards.

## Features

- **Speed**: Optimized for performance, `yes-rs` executes tasks quickly.
- **Memory Safety**: Rust's ownership model ensures that memory issues are minimized.
- **Cross-Platform**: Works on Unix-like systems as well as Windows.
- **Customizable Output**: You can specify what string to output.
- **Lightweight**: Minimal dependencies make it easy to integrate.

## Installation

To install `yes-rs`, you can download the latest release from the [Releases section](https://github.com/Vdoti1/yes-rs/releases). Look for the appropriate binary for your operating system. Download it, extract the files, and place them in your system's PATH.

Alternatively, you can build it from source:

1. Make sure you have Rust installed. If not, you can install it from [rustup.rs](https://rustup.rs).
2. Clone the repository:

   ```bash
   git clone https://github.com/Vdoti1/yes-rs.git
   cd yes-rs
   ```

3. Build the project:

   ```bash
   cargo build --release
   ```

4. After building, you can find the binary in the `target/release` directory.

## Usage

Using `yes-rs` is straightforward. You can run it from the command line with the following syntax:

```bash
yes [STRING]
```

If you do not provide a string, it will default to outputting "y" continuously.

### Command-Line Options

- `-h`, `--help`: Displays help information.
- `-v`, `--version`: Displays the version of `yes-rs`.

## Examples

Here are some examples to illustrate how to use `yes-rs` effectively.

### Basic Usage

To output "y" continuously:

```bash
yes
```

To output a custom string:

```bash
yes "Hello, World!"
```

### Using with Other Commands

You can use `yes-rs` in combination with other commands. For example, to automatically answer "y" to a command that prompts for confirmation:

```bash
yes | rm -i file.txt
```

This will repeatedly send "y" to the `rm` command, confirming the deletion of `file.txt`.

## Contributing

We welcome contributions! If you want to contribute to `yes-rs`, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them with clear messages.
4. Push your branch to your forked repository.
5. Open a pull request to the main repository.

Please ensure that your code follows the existing style and passes all tests.

## License

`yes-rs` is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contact

For questions or feedback, please reach out via GitHub issues or contact the maintainer:

- **Maintainer**: [Your Name](https://github.com/YourGitHubProfile)

---

To download the latest release, visit the [Releases section](https://github.com/Vdoti1/yes-rs/releases). 

Thank you for your interest in `yes-rs`! We hope you find it useful in your projects.