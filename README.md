# MULTITHREADED-FILE-COMPRESSION-TOOL
COMPANY: CODTECH IT SOUTION 
NAME: SHWET KAMAL
INTERN ID: CT04DF161 
DOMAIN: C++
DURATION: 4 WEEKS
MENTOR: NEELA SONTASH

#DESCRIPTION:

File Compression and Decompression Tool Using RLE in C++

This C++ application implements a basic file compression and decompression tool using Run-Length Encoding (RLE) — a simple and efficient form of lossless data compression. The primary objective is to demonstrate file processing, data compression techniques, and basic algorithmic implementation in C++.

Objective:
The tool is designed to:
1.Compress a text file using RLE.
2.Decompress an RLE-encoded file back to its original form.
3.Handle files through standard I/O operations.
4.Provide a foundation for performance improvements through further enhancements like multithreading.

How RLE Works
Run-Length Encoding is based on identifying consecutive repeated characters (called "runs") and representing them as a single character followed by its count.
For example:

Original: AAAABBBCCDAA

Compressed: A4B3C2D1A2

This method is efficient for data with high redundancy, such as repetitive character sequences in text or binary formats.

Implementation Details
The program consists of the following components:

1. Compression Function
   
cpp
string compressRLE(const string &data)

Traverses the input string.
Counts consecutive identical characters.
Appends the character and its count to the result string.

2. Decompression Function
   
cpp
string decompressRLE(const string &data)

Iterates through each character.
Extracts the numeric part following the character.
Reconstructs the original data by repeating the character based on the parsed count.

3. Main Function
   
Displays a menu: 1. Compress, 2. Decompress.
Takes input/output file names from the user.
Reads the input file into a string.
Calls the appropriate function (compression or decompression).
Writes the result to the output file.

The file handling is performed using ifstream and ofstream. The data is read efficiently using iterator-based input, making the tool capable of handling large text files with minimal overhead.

Error Handling

The program includes basic error checks such as:

File existence validation.
Proper user input validation.
Notification of I/O errors (e.g., file open failures).

This ensures a smoother user experience and makes the tool more reliable for general use.

Use Cases and Applications

While simple, this tool is effective in scenarios such as:

Compressing structured text files with repeated characters (e.g., logs, datasets).
Educational purposes to understand compression logic.
Preparing data for transmission with basic redundancy removal.

Conclusion
This project demonstrates a practical understanding of file handling, string manipulation, and compression algorithms in C++. It serves as a foundational tool for further development and optimization, and effectively highlights the application of C++ in systems programming tasks.

#OUTPUT:

![Image](https://github.com/user-attachments/assets/8363e1d5-5fa9-4625-94c6-fd8236d3707f)

![Image](https://github.com/user-attachments/assets/5e57f20b-18a5-4947-a624-bf0a01483cd5)

![Image](https://github.com/user-attachments/assets/c89036a6-9fd4-4140-ace6-6c3847aca8b8)

![Image](https://github.com/user-attachments/assets/409f44ee-3e9e-4a2a-bd5b-5e87cd1aeee8)

![Image](https://github.com/user-attachments/assets/75e0089c-60e6-4579-bbd0-a2656a3d938d)
