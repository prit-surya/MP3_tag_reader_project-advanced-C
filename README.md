MP3 Tag Reader

Introduction

MP3 Tag Reader is a desktop-based software application developed to read and display MP3 (ID3) tag information from MP3 files. It enables users to view metadata such as song title, artist, album, and more. This tool is designed to handle most ID3 versions, except ID3v2.4. In the future, it can be extended to implement editing capabilities for MP3 tags, making it a comprehensive MP3 metadata manager.


Features

Mandatory Features:
ID3 Version Support: Handles ID3v1, ID3v1.1, ID3v2, and ID3v2.3 (excluding ID3v2.4).

Metadata Display: Displays all metadata information available in the ID3 tag.

Version Display: Shows which version of ID3 tag is used in the MP3 file.

Help Menu: Provides a help screen (-h option) that details available options.

Embedded Image Support: If any image is embedded in the file, it displays information such as type, path, and size.

Error Handling: Displays proper error messages if no ID3 tag is found.


Additional Features:
Album Art Extraction: Option to extract album art from the file.

Tag Deletion: Option to delete all tag data or a selected tag from the file.

ID3v2.4 Support: Future support for ID3v2.4 version.

Tag Editor: Ability to edit the tags using command-line options.

Scope
This project aims to fully capture all the requirements for reading MP3 tags and help prepare a system architecture and design documents. It will be useful for individuals and developers looking to view or collect MP3 tag data. The project follows an object-oriented and modular design approach to make future expansion easier.

Development Environment

Programming Language: C

Interface: Command Line Interface (CLI)

Operating System: Linux (Ubuntu)

User Interface Requirements
Help Menu: Displays a help window with all options.

Metadata Information: Displays all MP3 metadata in the terminal.
Functional Requirements
Handle all ID3 versions except ID3v2.4.
Display the version of the ID3 tag.
Show all metadata details.
Provide the ability to edit tags through command-line options.
Display help screen on request using -h.
Display image details if an image is embedded in the MP3 file.
Proper error messages when no ID3 tag is found.
Design Guidelines
Object-oriented and modular code design.
Different modules for different functionalities for easy teamwork.
Clear communication and team effort.
Follow coding and testing guidelines.
Coding Guidelines
Use proper naming conventions for variables, functions, classes, etc.
Separate class definitions into headers and functions into .c files.
Comment the code adequately for better readability.
Do not hardcode values.
Testing Guidelines
Ensure comprehensive test cases are prepared to validate all functionalities.
The project is considered complete when all test cases pass successfully.


About MP3 ID3 Tags
ID3v1 & ID3v1.1: These tags are stored at the end of MP3 files and have a total size of 128 bytes.
ID3v2, ID3v2.3 & ID3v2.4: These tags are more flexible, usually located at the beginning of the MP3 file. They consist of a header and one or more frames.
For detailed information on ID3 tags, please refer to:

Wikipedia article on ID3 tag
ID3 tag standard website
ID3 tag version 2.3 standard
How to Run the Project on Linux (Ubuntu)
Compile the project:

bash
Copy code
gcc mp3_tag_reader.c -o a.out
To display help:

bash
Copy code
./a.out --help
To display MP3 tag information:

bash
Copy code
./a.out -v test.mp3
To edit the title tag:

bash
Copy code
./a.out -e -t title_name test.mp3




Author

Name: Pritesh Suryawanshi

Batch: ECEP (24002_030) - Emertxe

Guidance: Emertxe
