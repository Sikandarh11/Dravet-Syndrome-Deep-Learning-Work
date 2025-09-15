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
├── data/                # Instructions for obtaining data (see below)
├── CNN + LSTM/          # Scripts and notebooks for CNN + LSTM models
├── lstm gru/            # Scripts and notebooks for LSTM-GRU models
├── lstm/                # Scripts and notebooks for LSTM models
├── notebooks/           # Jupyter notebooks for exploratory analysis and modeling
├── scripts/             # Python scripts for data processing, model training, and evaluation
├── models/              # Saved models and checkpoints
├── utils/               # Utility functions and helper modules
├── requirements.txt     # List of package dependencies
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
   - Use provided scripts in the `scripts/` or notebooks in `notebooks/` for preprocessing.

2. **Model Training:**
   - There are three main model directories:
     - `CNN + LSTM/`
     - `lstm gru/`
     - `lstm/`
   - Refer to the scripts and notebooks within each directory for training different architectures.

   - Example command to train a model:
     ```bash
     python scripts/train.py --config configs/model_config.yaml
     ```
   - You can adjust parameters via the config files or command-line arguments.

3. **Evaluation:**
   - Run evaluation scripts to reproduce quantitative results:
     ```bash
     python scripts/evaluate.py --model models/best_model.pth
     ```

4. **Visualization:**
   - Use Jupyter notebooks in the `notebooks/` directory for exploratory data analysis and visualizations.

5. **Kaggle Notebooks:**
   - Recently added Kaggle notebooks are included in the repository.  
   - **Note:** You need to manually run these notebooks after obtaining the data as per the instructions above.

6. **Reproducing the Pipeline:**
   - Step-by-step instructions for reproduction are provided in `notebooks/` and the main scripts.
   - All random seeds are set where applicable to ensure reproducibility.

---

## Reproducibility Guidelines

- All code, including preprocessing, training, and evaluation, is included and documented.
- The code is version controlled and all dependencies are specified in `requirements.txt`.
- Scripts are modular and annotated for clarity.
- Results in the paper can be reproduced following the instructions above.
- For any issues, see [Contact](#contact).

---

## Dependencies

All dependencies are listed in `requirements.txt`. Main dependencies include:

- Python (>=3.7)
- NumPy
- pandas
- scikit-learn
- PyTorch or TensorFlow (depending on the model)
- matplotlib or seaborn
- jupyter

Install all dependencies with:

```bash
pip install -r requirements.txt
```

---

## requirements.txt Example

Below is a template for the `requirements.txt` file.  
**Update the version numbers and packages as necessary for your specific environment:**

```
numpy>=1.18.0
pandas>=1.0.0
scikit-learn>=0.22.0
torch>=1.7.0        # or tensorflow>=2.0.0 if you are using TensorFlow
matplotlib>=3.1.0
seaborn>=0.10.0
jupyter
```

---

## Code License

All code in this repository is available under the MIT License (see [LICENSE](LICENSE)).  
You are free to use, modify, and redistribute the code with appropriate attribution.

---

## Contact

For questions, clarifications, or requests for data access, please contact:

- **Sikandarh11** (Repository Owner)  
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
