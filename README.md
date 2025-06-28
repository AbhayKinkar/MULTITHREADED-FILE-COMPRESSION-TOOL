# MULTITHREADED-FILE-COMPRESSION-TOOL
COMPANY NAME: CODETECH IT SOLUTION

NAME: ABHAY KUMAR KINKAR

INTERN ID: CT04DF331

DOMAIN: C++

MENTOR: NEELA SANTOSH

#DISCRIPTION:
This C++ program demonstrates a simple implementation of Run-Length Encoding (RLE) for compressing and decompressing text data from files. Run-Length Encoding is a basic form of data compression where consecutive occurrences of the same character are stored as a single character followed by the number of times it appears. This is particularly useful in scenarios where data contains many repeated characters.

The program begins by including several essential header files: <iostream> for standard input/output operations, <fstream> for file handling, <string> for string manipulations, and <cctype> for checking character types like digits. The using namespace std; line allows the use of standard library elements without prefixing them with std::.

Two main functions form the core logic of this program: compressRLE and decompressRLE.

Compression Logic
The compressRLE function takes a string input and compresses it using the RLE algorithm. It initializes a result string to store the compressed output and uses a counter to keep track of repeated characters. The function iterates through the input string starting from the second character. If the current character is the same as the previous one, it increments the count. When a different character is encountered, it appends the previous character and its count to the result string. This process continues until all characters are processed, and finally, the compressed result is returned. For example, the string aaaabb would be compressed to a4b2.

Decompression Logic
The decompressRLE function performs the inverse operation. It takes a compressed string and reconstructs the original string. It iterates through each character of the input. If it encounters a character, it checks the following digits to find out how many times that character should be repeated. These digits are converted into an integer using stoi() and appended to the result string accordingly. This function is careful to handle multiple digits in the count (like 'a12'), using a while loop to build the full number.

Main Program Flow
The main function handles file input/output and user interaction. It begins by prompting the user to select either compression or decompression. The user must also provide the input file name and the desired output file name. The program then attempts to open the input file. If unsuccessful, it displays an error message and terminates.

If the file is opened successfully, the entire content is read into a string using stream iterators. Depending on the user’s choice, the program calls either compressRLE or decompressRLE to process the data. If the choice is invalid, the program notifies the user and exits.

After processing, the program attempts to open the output file to write the result. If it fails, an error is shown. Otherwise, the processed string is saved, and a success message is printed.


Summary
Overall, this program showcases a practical and simple example of text file compression and decompression using Run-Length Encoding in C++. It uses modern C++ features such as string manipulation, file streams, and iterators. Error handling is implemented for file access, and user input guides the program’s operation. While RLE is not suitable for all types of data due to its simplicity, it serves as an excellent educational example of how compression algorithms work and how they can be applied using fundamental programming constructs.


OUTPUT:

![Image](https://github.com/user-attachments/assets/ff789968-fa9d-4872-ab85-4ff86f2669ac)

![Image](https://github.com/user-attachments/assets/81c637b0-1b6c-4cbd-ba57-b1d62f506eaf)

![Image](https://github.com/user-attachments/assets/05a30db4-4a42-4c14-bf6b-020678ac4f21)

