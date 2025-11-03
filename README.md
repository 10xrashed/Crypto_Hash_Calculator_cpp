# Crypto Hash Calculator

A simple command-line utility written in C++ for generating various cryptographic hash values (MD5, SHA-1, SHA-256, SHA-512) for a given input string.

## Features

*   Calculates MD5 hash
*   Calculates SHA-1 hash
*   Calculates SHA-256 hash
*   Calculates SHA-512 hash
*   Colorized output for better readability
*   Easy-to-use command-line interface

## Prerequisites

To compile and run this program, you will need:

*   A C++ compiler (like g++)
*   OpenSSL development libraries (for cryptographic hash functions)

### Installing OpenSSL Development Libraries

**Debian/Ubuntu:**
```bash
sudo apt-get update
sudo apt-get install libssl-dev
```

**Fedora/RHEL/CentOS:**
```bash
sudo dnf install openssl-devel
```

**macOS (using Homebrew):**
```bash
brew install openssl
```
    *Note: You might need to add OpenSSL's include and lib directories to your compiler's search paths.*

## How to Compile

Navigate to the directory containing `hash_calculator.cpp` and compile using g++:

```bash
g++ hash_calculator.cpp -o hash_calculator -lcrypto -lssl
```

## How to Run

After successful compilation, execute the program:

```bash
./hash_calculator
```

The program will then prompt you to enter the text you wish to hash.

## Example Usage

```
======================================================================
  CRYPTOGRAPHIC HASH CALCULATOR
======================================================================

Enter text to hash: Hello World!

Input: "Hello World!"

Algorithm   Bits      Hash
----------------------------------------------------------------------
MD5         128       ed076287532e86365e841e92bfc50d8c
SHA-1       160       2ef7bde608ce5404e97d00f04fd9f13e025ff75e
SHA-256     256       7f83b1657ff1fc53b92dc18148a1d65dfc2d4b1fa3d677284addd200126d9069
SHA-512     512       861844d6704e8573fec34d967e20bcfef3d42498bd26797274079996fe11addc617b0754f04de8fe53927d048bb64d1f91c2b62b6628b73656bc86e2ddf82410

======================================================================
```

## Contributing

Feel free to fork this repository, open issues, or submit pull requests.

## License

This project is open-source and available under the [MIT License](LICENSE).
