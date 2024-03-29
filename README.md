# Password Manager

This program is a simple password manager developed in C++ with features for creating user accounts, logging in, and password cracking using MD5 and SHA256 hashing algorithms. The program utilizes OpenSSL for cryptographic functions.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [File Descriptions](#file-descriptions)
- [Building the Program](#building-the-program)
- [Testing](#testing)

## Installation

To use this program, you need to have OpenSSL installed. You can download OpenSSL from [OpenSSL Downloads](https://www.openssl.org/source/).

## Usage

### Admin Menu

The main menu provides administrative options:

1. **Create Account:** Create a new user account.
2. **Test Login:** Test user login with username and password.
3. **Password Cracker:** Access the password cracking menu.
4. **Exit:** Exit the program.

### Password Cracker Menu

The password cracker menu allows you to:

1. **Convert to MD5:** Convert a password to its MD5 hash.
2. **Convert to SHA256:** Convert a password to its SHA256 hash.
3. **Crack MD5 Hash:** Crack an MD5 hash and retrieve the original password.
4. **Crack SHA256 Hash:** Crack a SHA256 hash and retrieve the original password.
5. **Return:** Return to the main menu.

## File Descriptions

- **main.cpp:** Contains the main program and administrative menu functions.
- **user.cpp:** Implements user-related functions, including user creation and file I/O.
- **user.h:** Header file for the user class and related functions.
- **crack.cpp:** Implements password cracking functions using MD5 and SHA256.
- **crack.h:** Header file for password cracking functions.
- **test.cpp:** Contains Google Test-based unit tests for validating various functionalities of the program.
- **Makefile:** Makefile for building the program.
- **commonpasswordsMD5.txt:** File containing common passwords and their MD5 hashes.
- **commonpasswordsSHA256.txt:** File containing common passwords and their SHA256 hashes.

## Building the Program

To build the program, make sure you have OpenSSL installed. Modify the `Makefile` if necessary.

## Testing

This project uses Google Test for unit testing. The unit tests are defined in the `test.cpp` file, and the test executable is built using the Makefile. To run the tests, ensure that you have Google Test installed, and then use the following commands:

```bash
# Build and run the tests
mingw32-make test
```

Make sure to replace mingw32-make with make if you are using a different make tool.