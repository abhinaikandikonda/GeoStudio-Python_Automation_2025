# GeoStudio Python Automation (2025)

This repository contains the Python script developed for automating GeoStudio simulations. 
The script updates XML model files, runs multiple simulations using GeoCmd.exe, and saves the output results automatically. 
These instructions explain how to run the code on any computer.


## Instructions for Running the Automated Python Script

### 1. Update File Paths
Before running the script on a new PC, make sure all file paths inside the Python script are updated:
- Set the correct path for **GeoCmd.exe**.
- Update the path of the **Excel file** that contains material property values.
- Ensure the output directories (such as **xmlfiles**) are correctly defined.



## 2. Excel File Configuration
The script reads material properties directly from an Excel file. Ensure that:
- The Excel file is at the correct file path.
- The format, column names, and structure of the Excel file remain unchanged.



## 3. XML Model File Requirement
- The XML model file must be generated **before** running the script.
- This XML file defines the geometry and structure of the system.
- The script uses this XML template and updates the material properties for each simulation iteration.



## 4. Mesh File Requirement
- Ensure the required **mesh file** is present inside the **xmlfiles** directory.
- The simulation will not run if the mesh file is missing.



## 5. Output Directory Setup
Before running the script:
- Create an **xmlfiles** folder inside your output directory.
- This folder will store all intermediate XML files generated during the simulations.



## 6. Output Generation
Once the script is started, it will automatically:
1. Generate multiple XML input files by updating the material properties from the Excel file.
2. Execute each XML file using **GeoCmd.exe**.
3. Save the output results (Factor of Safety, etc.) in Excel format inside the output directory.



## Code Availability
This code is shared as part of the journal review process for transparency and reproducibility.
