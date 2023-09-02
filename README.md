# azazil_zip-slip_tool

azazil_zip-slip_tool is a powerful command-line tool written in Python that allows you to create archives with directory traversal, specifically designed to demonstrate path traversal vulnerabilities. This tool serves as an educational resource and helps raise awareness about security risks associated with improper handling of file paths.

## Features

- Create archives with customizable levels of directory traversal.
- Support for various archive types, including zip, jar, tar, tar.gz, tar.bz2, and tgz.
- Specify custom paths within the archive for greater flexibility.
- Choose between Windows or Unix platform for the archive.
- Useful for demonstrating security vulnerabilities and promoting secure coding practices.

## Installation

1. Ensure you have Python 3.11 installed on your system.
2. Clone the repository or download the "azazil_zip-slip_tool.py" file directly.
3. Open a terminal or command prompt and navigate to the directory where the tool is located.

## Usage

To use azazil_zip-slip_tool, follow these steps:

1. Run the program by executing the following command: `python azazil_zip-slip_tool.py [options] input_file`.

### Options

- `--output-file` or `-f`: Specifies the output file name and extension. Default: "AzaziL.zip".
- `--depth` or `-d`: Sets the number of directories to traverse. Default: 8.
- `--os` or `-o`: Specifies the OS platform for the archive. Options: "win" for Windows, "unix" for Unix-like systems. Default: "win".
- `--path` or `-p`: Sets the custom path within the archive. Default: No path added.

### Examples

Here are some examples of how to use azazil_zip-slip_tool:

1. Create a zip archive named "payload.zip" containing the file "payload.txt" with 5 levels of directory traversal:
   `````
   python azazil_zip-slip_tool.py -f payload.zip -d 5 payload.txt
   ```

2. Generate a tar archive named "data.tar" with the file "data.csv" using 3 levels of directory traversal:
   ````
   python azazil_zip-slip_tool.py -f data.tar -d 3 data.csv
   ````

3. Create a tar.gz archive named "backup.tar.gz" containing the file "backup.sql" with a custom path "database\backups\" and 5 levels of directory traversal:
   ````
   python azazil_zip-slip_tool.py -f backup.tar.gz -d 5 -p database\backups\ backup.sql
   ````

4. Create a jar archive named "malware.jar" containing the file "malware.exe" with the Unix platform and 10 levels of directory traversal:
   ````
   python azazil_zip-slip_tool.py -f malware.jar -d 10 -o unix malware.exe
   ````

5. Create a tgz archive named "archive.tgz" containing the file "data.txt" with the default options:
   ````
   python azazil_zip-slip_tool.py -f archive.tgz data.txt
   ````

6. Generate a jar archive named "app.jar" containing the file "App.class" with a custom path "com\example\" and 3 levels of directory traversal:
   ````
   python azazil_zip-slip_tool.py -f app.jar -d 3 -p com\example\ App.class
   ````

7. Create a zip archive named "images.zip" containing the files in the "images" directory with 4 levels of directory traversal:
   ````
   python azazil_zip-slip_tool.py -f images.zip -d 4 images/
   ````

8. Generate a tar.gz archive named "logs.tar.gz" containing all files in the "logs" directory with the Unix platform and 6 levels of directory traversal:
   ````
   python azazil_zip-slip_tool.py -f logs.tar.gz -d 6 -o unix logs/
   ````

9. Create a tar archive named "documents.tar" containing all files in the "documents" directory with the default options:
   ````
   python azazil_zip-slip_tool.py -f documents.tar documents/
   ````

10. Generate a jar archive named "code.jar" containing the files in the "src" directory with 2 levels of directory traversal:
    ```
    python azazil_zip-slip_tool.py -f code.jar -d 2 src/
    ```

Feel free to adjust the filenames, paths, and options to meet your specific requirements.

## Disclaimer

Please use this tool responsibly and only on systems for which you have proper authorization. The tool is intended for educational purposes and raising awareness about path traversal vulnerabilities. Be sure to adhere to ethicalhacking guidelines and obtain proper consent before using this tool.

## Contributing

Contributions are welcome! If you have any suggestions, bug reports, or feature requests, please open an issue or submit a pull request on the GitHub repository.

## Acknowledgements

Special thanks to the original author of the evilarc tool, which served as the foundation for this project.

## Contact

For any inquiries or further information, please contact [molcooteh@gmail.com](mailto:molcooteh@gmail.com).

We hope you find the azazil_zip-slip_tool useful and informative. Happy archiving!

*Please note that the examples provided demonstrate the functionality of the tool and path traversal vulnerabilities. It's crucial to use this tool responsibly and only on authorized systems.*
