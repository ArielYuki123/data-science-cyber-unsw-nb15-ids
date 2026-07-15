# Data Science in Cybersecurity Final Project: IDS on UNSW-NB15

## Project Description

This repository contains my final project for the Data Science in Cybersecurity course.

The project critically evaluates and reproduces a tutorial/article that builds an Intrusion Detection System using machine learning on the UNSW-NB15 dataset.

The objective is not only to reproduce the original results, but also to evaluate whether the author's claims are supported by the data, methodology, and experiments.

## Selected Source

Article/tutorial:
"Building an Intrusion Detection System on UNSW-NB15 Dataset Based on Machine Learning Algorithm" by Subrata Maji.
https://medium.com/%40subrata.maji16/building-an-intrusion-detection-system-on-unsw-nb15-dataset-based-on-machine-learning-algorithm-16b1600996f5

Original GitHub repository:
https://github.com/SubrataMaji/IDS-UNSW-NB15

## Dataset

Dataset:
UNSW-NB15 intrusion detection dataset.

Official dataset source:
https://research.unsw.edu.au/projects/unsw-nb15-dataset

The dataset is not included in this repository because of size considerations.
The full UNSW-NB15 CSV files should be downloaded separately and placed under `data/raw/`.

## Repository Structure

```text
notebooks/   Main project notebook
reports/     Final PDF report
figures/     Generated figures
data/        Local data directory, not tracked by Git
```

## Execution Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/ArielYuki123/data-science-cyber-unsw-nb15-ids.git
cd data-science-cyber-unsw-nb15-ids
```

### 2. Install Dependencies

Install the required Python packages:

```bash
pip install -r requirements.txt
```

The main dependencies used in this project are:

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
notebook
```

If running the project in Google Colab, most of these packages are already installed.

### 3. Download the Dataset

Download the full UNSW-NB15 CSV dataset from the official UNSW-NB15 dataset source.

The required files are:

```text
UNSW-NB15_1.csv
UNSW-NB15_2.csv
UNSW-NB15_3.csv
UNSW-NB15_4.csv
UNSW-NB15_features.csv
```

Place these files in the following local folder:

```text
data/raw/
```

The dataset files are not included in this GitHub repository because of their size.

### 4. Run the Notebook

Open the main notebook:

```text
notebooks/unsw_nb15_ids_project.ipynb
```

Run the notebook cells from top to bottom.

The notebook performs the following steps:

```text
1. Clone/reference the original GitHub repository used by the blog
2. Load the full UNSW-NB15 CSV dataset
3. Inspect the dataset structure, columns, feature types, and labels
4. Perform exploratory data analysis
5. Perform feature engineering and preprocessing
6. Train machine-learning models for binary intrusion detection
7. Evaluate the models using cybersecurity-relevant metrics
8. Perform error analysis
9. Summarize the findings
```

### 5. Expected Local Folder Structure

Before running the notebook, the project folder should look like this:

```text
PROJECT_ROOT/
│
├── README.md
├── requirements.txt
├── notebooks/
│   └── unsw_nb15_ids_project.ipynb
│
├── reports/
│   └── report.pdf
│
├── figures/
│
└── data/
    └── raw/
        ├── UNSW-NB15_1.csv
        ├── UNSW-NB15_2.csv
        ├── UNSW-NB15_3.csv
        ├── UNSW-NB15_4.csv
        └── UNSW-NB15_features.csv
```

### 6. Output Files

During execution, the notebook may generate processed data files, figures, model results, or evaluation tables. These files may be saved under:

```text
data/processed/
figures/
results/
```

The `data/` folder is intended for local use only and should not be uploaded to GitHub.

### 7. Reproducibility Notes

The project uses fixed random seeds where appropriate, such as `random_state=42`, to make train/test splitting and model training more reproducible.

The notebook was designed to reproduce and critically evaluate the methodology of the selected blog post using the full UNSW-NB15 CSV dataset.
