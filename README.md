# Dravet-Syndrome-Deep-Learning-Work

## Overview

This repository contains all scripts, code, and data processing pipelines developed for our research on the application of deep learning methods to Dravet Syndrome-related data. The repository is structured to facilitate reproducibility and ease of use for researchers and practitioners interested in this domain.

---

## Table of Contents

- [Project Description](#project-description)
- [Repository Structure](#repository-structure)
- [Installation & Setup](#installation--setup)
- [Data Availability](#data-availability)
- [Usage Instructions](#usage-instructions)
- [Reproducibility Guidelines](#reproducibility-guidelines)
- [Dependencies](#dependencies)
- [Code License](#code-license)
- [Contact](#contact)
- [Citation](#citation)
- [Acknowledgements](#acknowledgements)
- [Compliance with PLOS ONE Guidelines](#compliance-with-plos-one-guidelines)

---

## Project Description

This project explores and implements deep learning algorithms for the analysis of data related to Dravet Syndrome, a severe form of epilepsy. The codebase includes model architectures, training scripts, evaluation routines, and utility functions to support the full pipeline from raw data to results. Notebooks for exploratory analysis and modeling are included, and all code is version controlled for reproducibility.

---

## Repository Structure

```
Dravet-Syndrome-Deep-Learning-Work/
├── 1. CNN + LSTM/           # CNN + LSTM model notebook and trained model
│   ├── deep-learning-cnn-lstm-v4.ipynb
│   └── trained_model.h5
├── 2. LSTM/                 # LSTM model notebook and trained model
│   ├── lstm-v1.ipynb
│   └── trained_model_lstm_fc.h5
├── 3. LSTM + GRU/           # LSTM-GRU model notebook and trained model
│   ├── deep-learninglstm-gru-v1.ipynb
│   └── trained_model_lstm_gru.h5
├── requirements.txt         # List of package dependencies
├── LICENSE
└── README.md
```

---

## Installation & Setup

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Sikandarh11/Dravet-Syndrome-Deep-Learning-Work.git
   cd Dravet-Syndrome-Deep-Learning-Work
   ```

2. **Set up the environment:**

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```

---

## Data Availability

> **Note:** Due to privacy/ethical restrictions, raw data are not included in this repository.  
> The `data/` folder will contain a README with a link to download the data from Google Drive.  
> Anyone with the link will be able to download the data. Please follow the instructions in `data/README.md` to access and prepare the data for use.

---

## Usage Instructions

1. **Data Preparation:**
   - Download the data using the link provided in `data/README.md` and follow the instructions there to place it correctly.
   - Each notebook contains data preprocessing steps within the notebook itself.
   - **Important:** You need to adjust the data paths in each notebook according to your local setup:
     ```python
     # Example paths that need to be updated in notebooks:
     control_folder = '/kaggle/input/my-dataset/Dataset/Control EEG'
     ds_folder = '/kaggle/input/my-dataset/Dataset/DS cases'
     
     # Update these paths to match your local data directory structure
     ```

2. **Model Training and Evaluation:**
   Each directory contains a complete Jupyter notebook with the full pipeline:
   
   - **CNN + LSTM Model:** Open and run `1. CNN + LSTM/deep-learning-cnn-lstm-v4.ipynb`
   - **LSTM Model:** Open and run `2. LSTM/lstm-v1.ipynb`
   - **LSTM + GRU Model:** Open and run `3. LSTM + GRU/deep-learninglstm-gru-v1.ipynb`

   Each notebook includes:
   - Data loading and preprocessing
   - Model architecture definition
   - Training pipeline with hyperparameters
   - Model evaluation and metrics
   - Visualization of results
   - Model saving/loading functionality

3. **Using Pre-trained Models:**
   - Each directory contains a pre-trained model file (`.h5` format)
   - Load the models directly in the notebooks or use them for inference
   - Model loading code is included within each respective notebook

4. **Running the Notebooks:**
   ```bash
   # Start Jupyter notebook server
   jupyter notebook
   
   # Navigate to the desired model directory and open the notebook
   # Before running: Update data folder paths in the notebook cells
   # Run all cells to reproduce the complete pipeline
   ```

5. **Path Configuration:**
   - Before running any notebook, locate the data path variables and update them:
     ```python
     # Find these lines in each notebook and update paths:
     control_folder = 'your/local/path/to/Dataset/Control EEG'
     ds_folder = 'your/local/path/to/Dataset/DS cases'
     ```

---

## Reproducibility Guidelines

- **Complete Pipeline in Notebooks:** Each Jupyter notebook contains the entire pipeline from data loading to model evaluation, ensuring full reproducibility.
- **Pre-trained Models:** Trained models are included in each directory for immediate use and result verification.
- **Environment Setup:** All dependencies are specified in `requirements.txt` with version constraints.
- **Self-contained Notebooks:** Each notebook is designed to be run independently with all necessary code included.
- **Random Seeds:** Random seeds are set within each notebook to ensure reproducible results.
- **Step-by-step Execution:** Notebooks are organized with clear cell-by-cell execution for easy reproduction.

**To Reproduce Results:**
1. Set up the environment using `requirements.txt`
2. Obtain the data as per instructions
3. Open any of the three model notebooks
4. **Update data folder paths** in the notebook cells to match your local setup
5. Run all cells sequentially
6. Compare results with the pre-trained models provided

**For any issues with reproduction, see [Contact](#contact).**

---

## Dependencies

All dependencies are listed in `requirements.txt`. Main dependencies include:

- Python (>=3.7)
- NumPy
- pandas
- scikit-learn
- TensorFlow/Keras
- matplotlib
- seaborn
- jupyter

Install all dependencies with:

```bash
pip install -r requirements.txt
```

---

## Code License

All code in this repository is available under the MIT License (see [LICENSE](LICENSE)).  
You are free to use, modify, and redistribute the code with appropriate attribution.

---

## Contact

For questions, clarifications, or requests for data access, please contact:

- **Sikandar Hussain** (Repository Owner)  
  GitHub: [Sikandarh11](https://github.com/Sikandarh11)  
  Email: sikandarnust1140@gmail.com

---

## Citation

If you use this code or models in your research, please cite:

```
@software{Sikandarh11_dravet_dl,
  author = {Sikandarh11},
  title = {Dravet-Syndrome-Deep-Learning-Work},
  year = {2025},
  url = {https://github.com/Sikandarh11/Dravet-Syndrome-Deep-Learning-Work}
}
```

---

## Acknowledgements

We acknowledge all contributors and the open-source community for their tools and datasets.

---

## Compliance with PLOS ONE Guidelines

- The code is openly accessible and version controlled.
- Sufficient documentation is provided to allow others to reuse and reproduce results.
- Code is licensed for reuse.
- Data access instructions are provided.
- Contact information is included for queries regarding the code and data.
