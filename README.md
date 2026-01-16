# ELISA Plate Layout Generator for Pre-Dilution Templates

## Overview

This project is a **Python-based ELISA plate layout generator** designed to automate **pre-dilution and plate mapping** for commercial ELISA kits, specifically **IDvet** and **Biochek** templates.

It eliminates manual errors associated with Excel-based dilution calculations and ensures **standardized, reproducible 96-well plate layouts** for laboratory diagnostics.

The tool generates structured layouts that align with **kit manufacturer templates**, making it suitable for:

* Diagnostic laboratories
* Veterinary and biomedical laboratories
* Research laboratories running high-throughput ELISA assays


## Key Features

* Automated ELISA **96-well plate layout generation**
* Supports **pre-dilution workflows**
* Compatible with **IDvet** and **Biochek** ELISA kits
* Excel-based input/output for easy laboratory adoption
* Batch files (`.bat`) for **non-technical users**
* Reduces calculation errors and improves reproducibility


## File-by-File Explanation

### 1. Python Scripts

#### `Biochek template calculator template.py`

* Core Python script for generating **Biochek ELISA plate layouts**
* Reads structured Excel input
* Performs dilution logic and plate mapping
* Outputs a ready-to-use ELISA template

#### `IDvet template calculator.py`

* Core Python script for **IDvet ELISA kits**
* Implements kit-specific layout rules
* Ensures compliance with IDvet plate configuration standards



### 2. Batch Files (Windows Execution)

#### `Biochek template calculator.bat`

* Allows **double-click execution** of the Biochek script
* Designed for laboratory staff with no Python experience

#### `IDvet template calculator.bat`

* Same function as above but for IDvet templates
* Automatically launches the correct Python script



### 3. Data Directory

#### `data/`

Contains Excel templates required by the scripts.

##### `Biochek template calculator template.xlsx`

* Input/output Excel template for Biochek assays
* Defines plate structure, controls, and dilution pattern

##### `IDvet template calculator template.xlsx`

* Input/output Excel template for IDvet assays
* Pre-formatted according to manufacturer layout



### 4. Configuration & Metadata

#### `.gitignore`

* Prevents unnecessary or sensitive files from being tracked by Git

#### `LICENSE`

* Defines legal permissions and usage terms for the project

#### `.idea/`

* IDE configuration files (PyCharm)
* Not required for execution
* Can be safely ignored by users



## Requirements

* Python 3.8 or higher
* Windows OS (for `.bat` execution)
* Required Python libraries:

  * `pandas`
  * `openpyxl`
  * `numpy`

Install dependencies using:

bash
pip install pandas openpyxl numpy




## How to Use

### Option 1: For Non-Technical Users (Recommended)

1. Open the `data` folder
2. Fill in the appropriate Excel template:

   * Biochek → `Biochek template calculator template.xlsx`
   * IDvet → `IDvet template calculator template.xlsx`
3. Double-click the corresponding `.bat` file
4. The processed ELISA plate layout will be generated automatically



### Option 2: Command Line Execution

bash
python "Biochek template calculator template.py"


or

bash
python "IDvet template calculator.py"




## Use Cases

* Veterinary ELISA diagnostics
* Poultry disease surveillance
* Laboratory automation
* Quality-controlled assay preparation
* High-throughput testing environments



## Future Improvements

* GUI interface for broader usability
* Support for additional ELISA manufacturers
* CSV input/output support
* Validation logs for QA/QC documentation



## Author

**Muhammad Abubakar**
Laboratory Scientist | Microbiologist | Data & Automation Enthusiast



## License

This project is licensed under the terms defined in the `LICENSE` file.

Tell me how far you want to take it.
