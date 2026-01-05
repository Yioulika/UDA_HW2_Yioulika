============================================================
README – Final Project
MATH70103: Unstructured Data Analysis – MLDS
============================================================

COURSE / ASSESSMENT INFORMATION
------------------------------------------------------------
Module Title      : MATH70103 – Unstructured Data Analysis (MLDS)
Assessment Title  : Final Project
Academic Year     : Autumn 2025–2026
Instructor        : Dr. Anthea Monod
Institution       : Imperial College London

Student Name      : Yioulika Antoniades
Student CID       : 06035552
Submission Date   : 05 January 2026


OVERVIEW
------------------------------------------------------------
This project implements a hierarchical–conditional food
inspection pipeline using two Convolutional Neural Network
(CNN) models built entirely from scratch.

Model 1:
- A Hierarchical Multi-Head CNN
- Classifies whether the input product is:
    (a) Fresh Produce
    (b) Animal Protein
- If Fresh Produce:
    - Further classifies into Fruit or Vegetable
- If Animal Protein:
    - Further classifies into Seafood or Meat & Poultry
- Finally identifies the specific product type

Model 2:
- A Singular Multi-Head CNN
- Operates conditionally on Model 1 outputs
- Applies only to the following fruit classes:
    - Apples
    - Bananas
    - Mangos
    - Grapes
- Classifies product condition as:
    - Fresh
    - Rotten
    - Formalin-mixed


PACKAGE CONTENTS (ZIP FILE)
------------------------------------------------------------
The submission is provided as a ZIP file.

After extraction, the contents will include:
- UDAHW2_Code.ipynb
- README.txt
- UDA_Datasets (folder)


EXPECTED FOLDER STRUCTURE
------------------------------------------------------------
After extracting the ZIP file, the directory structure should
be as follows:

(Extracted Folder)/
├── UDAHW2_Code.ipynb
├── README.txt
└── UDA_Datasets/
    ├── Dataset1_Classes/
    ├── Dataset2_FruitCond/
    └── Image Samples/


IMPORTANT INSTRUCTIONS (READ CAREFULLY)
------------------------------------------------------------

STEP 1: Download and extract
-----------------------------------------
1. Download the provided ZIP file.
2. Extract (unzip) the contents to your local machine.
3. Confirm that the following are present:
   - UDAHW2_Code.ipynb
   - README.txt
   - UDA_Datasets (folder)


STEP 2: Open the notebook
-----------------------------------------
Open the file:

    UDAHW2_Code.ipynb

using Jupyter Notebook, JupyterLab, VS Code, or an equivalent
environment.


STEP 3: Set Dataset 1 Path (Model 1)
-----------------------------------------
Locate the FIRST code block titled:

"Hierarchical Multi-Head CNN Model for Food Classification
(Fresh Produce vs Animal Protein)"

Then:
1. Navigate to:
       UDA_Datasets → Dataset1_Classes
2. Right-click the folder and select "Copy as path"
3. Paste the copied path into the designated line in the first
   code block.

Example path (for reference only):

    C:\Users\Yioulika Antoniades\Desktop\UDA_Datasets\Dataset1_Classes

Code placeholder:

    DATASET1_PATH = "________________________________________"


STEP 4: Set Dataset 2 Path (Model 2)
-----------------------------------------
Locate the SECOND code block titled:

"Singular Multi-Head CNN Model for Food Condition
(Fresh / Rotten / Formalin-mixed)"

Then:
1. Navigate to:
       UDA_Datasets → Dataset2_FruitCond
2. Right-click the folder and select "Copy as path"
3. Paste the path into the designated line in the second code
   block.

Example path (for reference only):

    C:\Users\Yioulika Antoniades\Desktop\UDA_Datasets\Dataset2_FruitCond

Code placeholder:

    DATASET2_PATH = "________________________________________"


STEP 5: Set Image Path (Final Inference)
-----------------------------------------
Locate the THIRD code block titled:

"Hierarchical–Conditional Food Inspection System"

Then:
1. Navigate to:
       UDA_Datasets → Image Samples
       (or any valid test image within Dataset1_Classes)
2. Select ONE image file
3. Right-click the image → "Copy as path"
4. Paste the copied path into the designated line in the third
   code block.

Example path (for reference only):

    C:\Users\Yioulika Antoniades\Desktop\UDA_Datasets\Dataset1_Classes\
    test\Animal Protein\Seafood\Fish\Fish_Test_3.jpg

Code placeholder:

    IMAGE_PATH = "________________________________________"


STEP 6: Run the notebook
-----------------------------------------
After all paths are correctly set:

- Run ALL cells from top to bottom
- Do not skip any cells
- Ensure each cell executes without errors before proceeding


EXECUTION ENVIRONMENT
------------------------------------------------------------
The notebook was developed and tested using Python within a
standard Jupyter Notebook environment and relies on commonly
used scientific and deep learning libraries.


EXPECTED RUNTIME
------------------------------------------------------------
Total execution time may range from several minutes to longer,
depending on hardware capabilities and dataset loading time.


EXPECTED OUTPUT
------------------------------------------------------------
The notebook outputs classification and condition predictions
for the provided datasets and selected image sample, with
results displayed directly within the notebook cells.


NOTES / IMPORTANT REMINDERS
------------------------------------------------------------
- Folder and file names must not be changed.
- Absolute paths must be used.
- Incorrect paths will result in runtime errors.
- The notebook assumes datasets are structured exactly as
  provided.


END OF README
------------------------------------------------------------
