# cpp-file-compression-decompression
A basic command-line application written in C++ that uses run-length encoding to compress and decompress text files.

## Overview

This repository contains a simple command-line tool, written in C++, for compressing and decompressing text files using run-length encoding (RLE). This tool demonstrates file I/O, string manipulation, and exception handling in C++.

## Features

*   **Text File Compression:** Compresses a text file using run-length encoding, reducing file size by representing repeating characters with a character and count.
*   **Text File Decompression:** Decompresses a previously compressed text file using run-length decoding, restoring original content.
*   **Command-Line Interface:** Provides a basic text-based interface for selecting compression and decompression.
*   **File Type Check:** Verifies that the source file is a `.txt` file.
*   **Basic Error Handling:** Includes exception handling for cases like invalid input and file errors.

## Project Structure

The project consists of the following files:

*   `main.cpp`: Contains the main function, menu, and the core logic for compression and decompression.
*   `data.txt`: A sample text file that can be used as a source to be compressed.

## How the System Works:

1.  **Run-Length Encoding (RLE):**
    *   RLE is a simple form of data compression that represents repeating sequences of characters with a single character and a count of how many times it appears. For example, "AAABBBCC" becomes "A3B3C2".

2.  **Compression:** The `encodeString` function iterates over the input string, identifies runs of repeating characters, and creates the RLE encoded output.

3.  **Decompression:** The `decodeString` function takes the RLE-encoded string, extracts the character and count, and reconstructs the original string.

4.  **File Input/Output:** The system reads from and writes to files using C++ file streams (`ifstream` and `ofstream`).
