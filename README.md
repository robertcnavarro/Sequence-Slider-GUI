# Sequence-Slider-GUI
The Sequence Slider GUI is a Python-based application designed to facilitate
protein structure analysis and amino acid sequence prediction. It integrates the
SEQUENCE SLIDER tool with machine learning (ML) models to process crystal-
lographic data from PDB and MTZ files, predict amino acid sequences, and visu-
alize results through sequence logos and interactive HTML visualizations. The
application provides a user-friendly graphical interface built with Tkinter, mak-
ing it accessible to researchers and scientists in structural biology.
The tool supports two ML model types:
• Model 1 (without Consurf): Uses structural and energetic features for pre-
dictions.
• Model 2 (with Consurf): Incorporates conservation scores from Consurf
for enhanced predictions.
Overview
The Sequence Slider GUI is a Python-based application that integrates protein structure analysis with machine learning predictions. It provides a user-friendly interface for running the SEQUENCE SLIDER tool, processing its output, and applying machine learning models to predict amino acid sequences.

System Requirements
Linux operating system

Python 3.6 or higher

Tkinter (usually included with Python)

The following Python packages:

pandas

numpy

matplotlib

scikit-learn

xgboost

logomaker

Installation
Clone or download the repository containing the script

Install required Python packages:

bash
pip install pandas numpy matplotlib scikit-learn xgboost logomaker
Usage
Run the application:

bash
python gui_vertion2025Amayo_run_model2.py
The main GUI window will appear with the following sections:

Input Selection
Load PDB: Select a Protein Data Bank file (.pdb)

Load MTZ: Select an MTZ file containing crystallographic data

Process Execution
Run SEQUENCE SLIDER: Execute the SEQUENCE SLIDER analysis on loaded files

Prepare Data for ML Model: Process the results for machine learning model input

Machine Learning Actions
Load ML Model: Choose between two pre-trained models (with/without Consurf)

Run ML Model: Execute predictions using the loaded model

Plot Result: Visualize the prediction results

Load Consurf Result: Load conservation scores for enhanced predictions

Output Display
The bottom panel shows:

Text output of all operations

Interactive sequence logos of prediction results

Features
Processes protein structure data through SEQUENCE SLIDER pipeline

Integrates with pre-trained XGBoost machine learning models

Generates sequence logos showing predicted amino acids

Creates interactive HTML visualizations of protein sequences

Supports both models with and without Consurf conservation data

Automatically saves FASTA files of predicted sequences

File Outputs
The application generates several output files:

Processed data CSV files

Sequence logo images (JPG format)

FASTA files of predicted sequences

Interactive HTML visualizations

Log files documenting all operations

Troubleshooting
Ensure all required Python packages are installed

Verify input files are in correct formats

Check the log file (sequence_slider.log) for error messages

Make sure you have write permissions in the output directory

Notes
The application requires the SEQUENCE SLIDER tool (SLIDER_VENOM.py) to be present in a slider-master subdirectory

Pre-trained models should be in the specified subdirectories:

model_without_consurf_C/

model_consurf_C/

get READMED to dowload
Here's a concise README.md file formatted for easy downloading and use on Linux systems:

markdown
# Sequence Slider GUI Tool

## Quick Install & Run

```bash
# 1. Install dependencies
sudo apt-get install python3-tk  # For Tkinter GUI support
pip install pandas numpy matplotlib scikit-learn xgboost logomaker

# 2. Download the script
wget https://example.com/path/to/gui_vertion2025Amayo_run_model2.py

# 3. Run the application
python3 gui_vertion2025Amayo_run_model2.py
Requirements
Linux (Tested on Ubuntu 20.04/22.04)

Python 3.6+

Required Python packages:

pandas numpy matplotlib scikit-learn xgboost logomaker
Key Features
🧬 Protein structure analysis pipeline

🤖 Built-in machine learning models

📊 Interactive sequence visualization

💾 Automatic FASTA file generation

Input Files Needed
PDB file (.pdb)

MTZ file (.mtz)

(Optional) Consurf CSV for enhanced predictions

Troubleshooting
If you get errors about missing packages:

bash
pip install --upgrade pip
pip install <missing-package-name>
For Tkinter errors:

bash
sudo apt-get install python3-tk
Support
Contact: bioinformatics-support@example.com
Documentation: Full Documentation Link


### How to Use This README:
1. Copy this text
2. Save as `README.md` in your project directory
3. Users can view it with:
   ```bash
   cat README.md
or

bash
less README.md
The markdown format makes it:

Easy to read in terminal

Compatible with GitHub/GitLab

Simple to convert to HTML/PDF if needed

