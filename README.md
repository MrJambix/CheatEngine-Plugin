Array and Pointer Scanner

A powerful tool for scanning arrays and pointers in memory, designed for game hacking and reverse engineering.

Features

Scan for arrays and pointers in memory
Generate Cheat Engine tables (.CT files) for easy use
Support for multiple pointer chains and offsets
Fast and efficient scanning algorithm
Easy to use and customize
Usage

Clone the repository and build the project using Visual Studio or your preferred IDE.
Run the tool and select the process you want to scan.
Choose the scan options and click "Scan" to start the scanning process.
The tool will generate a Cheat Engine table file (.CT file) with the found arrays and pointers.
Requirements

Windows 10 or later
Visual Studio 2019 or later (for building the project)
Cheat Engine (for using the generated .CT files)
Contributing

If you'd like to contribute to this project, please fork the repository and submit a pull request with your changes. Make sure to follow the coding standards and guidelines outlined in the repository.

License

This project is licensed under the MIT License. See the LICENSE file for more information.

Acknowledgments
Thanks to the Cheat Engine community for their support and feedback.

Known Issues

I hope this helps! Let me know if you have any questions or need further assistance.


1. Create a new C++ project in Visual Studio.
2. Add the ArrayFinderPlugin.cpp and ArrayFinderTool.cpp files to the project.
3. Link against the Cheat Engine API library (CheatEngine.lib).
4. Build the project to create a DLL file (ArrayFinderPlugin.dll).
5. Open Cheat Engine and go to the "Plugins" menu.
6. Click "Load Plugin" and select the ArrayFinderPlugin.dll file.
7. The plugin should now be loaded and available in the "Plugins" men

**Memory Scanning**

The tool starts by scanning the game's memory for potential array patterns.
It uses the ReadProcessMemory function to read the memory contents of the game process.
The tool scans the memory in chunks, typically 4KB or 8KB at a time, to reduce the amount of data that needs to be processed.
Pattern Recognition

Once the tool has scanned the memory, it uses pattern recognition algorithms to identify potential array patterns.
The tool looks for sequences of values that are consistent with the expected pattern of an array.
The tool uses a combination of techniques, such as:
Checking for sequential values (e.g., 1, 2, 3, ...).
Checking for constant values (e.g., all zeros or all ones).
Checking for patterns of increasing or decreasing values.

**Data Extraction**

Once the tool has identified a potential array pattern, it extracts the relevant data from the memory.
The tool uses the ReadProcessMemory function to read the memory contents of the game process.
The tool extracts the data in chunks, typically 4 bytes or 8 bytes at a time, depending on the data type.

**Data Processing**

The tool processes the extracted data to determine the array's properties, such as its length and element size.
The tool uses algorithms to analyze the data and determine the array's structure.
The tool may also perform additional processing, such as filtering out invalid data or handling edge cases.

**Data Display**

Finally, the tool displays the extracted data in a user-friendly format.
Provide additional information, such as the array's address, length, and element size.
