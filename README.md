# AI-ML-Final-Proj

Installation

  1)Install Python 3.9 or newer.
  
  2)Install required packages:
  
    pip install torch torchvision timm scikit-learn pandas numpy matplotlib pillow tqdm openpyxl

Setup

  1)Clone or download this repository to your local machine.
  
  2)Ensure the following paths exist inside the repo (or update paths in the code to match):
  
    The cervical images folder containing per-case subfolders.
    
    The metadata Excel file in the repository root or a data/ folder.
    
  3)Confirm that case subfolders and filenames ending in 1 (e.g. AFC1.jpg, AJL1.jpg) are present and unchanged.
  
  4)Open the notebook file in Jupyter, VS Code, or Google Colab.


Configuration

  1)In the first configuration cell of the notebook, set IMG_ROOT to the folder containing the case subfolders.
  
  2)Set META_PATH to the full path of the metadata Excel file.
  
  3)Set OUT_DIR to a desired output folder.
  
  4)Leave all other hyperparameters (epochs, learning rate, image size) as provided to reproduce the original results.
  

Running the Notebook

  1)Run all cells in order from top to bottom without skipping any.
  
  2)Wait for training to complete for all epochs.
  
  3)After training, run the evaluation and statistics cells at the end of the notebook.
  
  4)Confirm that model checkpoints, metrics, and plots are created inside OUT_DIR and its subfolders.
  

Reproducing Results

  1)Use the generated plots for loss, accuracy, sensitivity, precision, recall, F1, ROC curves, and confusion matrices in OUT_DIR to match the original figures.
  
  2)Use the exported tables or printed statistics in the notebook output to match the reported accuracy, F1, sensitivity, and other metrics.
  
  3)If you need identical runs, keep the default random seed values in the notebook unchanged.


External Image Testing

  1)Place external cervix images in a new folder inside the repository.
  
  2)In the “external testing” or Grad-CAM section of the notebook, set the path to that folder.
  
  3)Run the corresponding cells to generate VIA predictions and Grad-CAM heatmaps for those images.
