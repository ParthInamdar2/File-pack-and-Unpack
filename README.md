# File-pack-and-Unpack

This project implements a command-line based File Packing and Unpacking system in Java, designed to combine multiple files into a single packed file and extract them later using custom logic.

Features:
- Pack multiple files into one single file
- Unpack the packed file and restore original files
- Uses custom header format (file name + file size)
- Command-Line Interface (CLI)
- Exception handling and robust Java I/O logic

Supported File Formats

- .txt
- .jpeg
- .docx

Technologies Used
- Core Java
- File Handling
- BufferedInputStream / BufferedOutputStream
- Object-Oriented Design
- Scanner & Exception Handling

How It Works (Logic)

➡ Packing Logic
  
 - Read each file inside the directory
 - Create a 100-byte header → "FullPath Size"
 - Write header + file data to output file
 - Repeat for all supported files

➡ Unpacking Logic

- Read 100-byte header
- Extract FileName and Size from header
- Create a new file using extracte
- Write file content according to size


🖥️ Usage / Commands

1️⃣ Run the Program
- javac Main.java
- java Main


➡ Packing Process


<img width="662" height="525" alt="image" src="https://github.com/user-attachments/assets/03b3003d-9773-4be8-acae-c50acdb921a4" />

➡ Unpacking Process

<img width="543" height="527" alt="image" src="https://github.com/user-attachments/assets/0568e2e1-e551-4c55-b054-bc621dbaf622" />



