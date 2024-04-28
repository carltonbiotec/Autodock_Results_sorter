# Autodock_Results_sorter
AutoDock Vina Results Processor
This Python application provides a graphical user interface (GUI) to facilitate the processing of AutoDock Vina docking simulation results. The tool is designed to help researchers quickly and efficiently extract the best docking scores from multiple output log files in text format, saving the results into a CSV file for further analysis.

Features
Folder Selection: Users can easily browse and select a folder containing AutoDock Vina log files.
Data Extraction: Automatically parses each text file in the selected folder to extract the best docking score, specifically the first mode which typically represents the best score.
CSV Output: Allows users to choose the save location and name for the resulting CSV file, which includes detailed information such as the file name, affinity in kcal/mol, and RMSD values.
How It Works
Browse and Select Folder: The GUI includes a button to browse and select the directory containing the .txt output files from AutoDock Vina.
Process Files: The script reads each text file, searching for the section that begins with "mode | affinity" to start extracting docking scores. It specifically captures the first mode entry as it represents the best docking score.
Save Results: After processing, users are prompted to save the extracted data to a CSV file. The file will include columns for File Name, Affinity (kcal/mol), RMSD LB, and RMSD UB.
Usage
Simply run the script in a Python environment with GUI support (e.g., Tkinter installed). Click the "Browse Folder" button to select the folder with your AutoDock Vina results and then choose where to save the CSV after the files have been processed.

Requirements
Python 3.x
Pandas
Tkinter


Installation
Clone the repository and install the required Python packages:

pip install pandas
python auto_dock_vina_processor.py
