# DS 4002 Project 3

## Software and Platform
We ran the scripts using VSCode using Windows on an NVIDIA GPU. We also used the following Python packages that can be installed using pip:
- matplotlib
- pandas
- pathlib
- seaborn

## Documentation Map
DS4002PROJECT3
- `README.md`: This file
- `LICENSE`: Description of the license for this project
- 📁 DATA Folder: contains data used throughout the pipeline
  - `METADATA.md`: Description of the data being used
  - 📁 `images`: Folder of all raw pet images, named in the format `breed_number`
  - `list.txt`: Raw space-separated-value text file containing image filenames and their corresponding species and breed labels
- 📁 OUTPUT Folder
  - `images_per_class.png`: Bar chart of number of images for each species (cat and dog)
  - `images_per_species.png`: Bar chart of number of images for each breed (37 total)
  - `species_confusion_matrix.png`: Confusion matrix of the CNN's performance in classifying cat vs. dog images
  - `results.md`: Formatted Markdown file summarizing and interpreting the results of the analysis
- 📁 SCRIPTS Folder
  - `0_processing.py`: Initial processing script to parse image annotations and generate exploratory plots
  - `1_cnn.py`: full CNN training pipeline (baseline model, augmented model, and 37-class model) 

## How to Reproduce Results
You can run the project in two steps:  
- `0_processing.py`: preprocessing and preliminary visualization of data
- `1_cnn.py`: trains the binary CNN (cat vs. dog), trains the augmented CNN, trains the 37-class breed CNN, and generates confusion matrices and evalution metrics
