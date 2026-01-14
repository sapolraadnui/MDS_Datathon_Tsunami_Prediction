# Tsunami Prediction (MDS Datathon)

This repository contains code, notebooks, and artifacts for a tsunami
prediction datathon project.

## Repository structure
``` bash
.
├── LICENSE
├── README.md
├── data/
│   ├── raw/                  Raw Kaggle data (train/test/sample_submission)
│   └── sample/               Small sample data (optional)
├── notebooks/                Exploration and experiments
├── reports/                  PDF writeup / report
├── requirements.txt          Python dependencies
├── src/
│   └── tsunami_prediction/   Reusable Python code (package)
└── submissions/              Submission CSVs
```
## Data

Place the Kaggle files in:

- data/raw/train.csv
- data/raw/test.csv
- data/raw/sample_submission.csv

Note:
If this repository is public, it is recommended NOT to commit raw data.
Use .gitignore to exclude data/raw/.

## Environment and dependencies

Using venv:

python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

Using conda / miniforge:

conda create -n tsunami python=3.12
conda activate tsunami
pip install -r requirements.txt

## Running the project

If the notebook logic has been refactored into Python modules under src/,
run:

PYTHONPATH=src python -m tsunami_prediction.train
PYTHONPATH=src python -m tsunami_prediction.predict

## Notebooks

Main notebook:
- notebooks/datathon_tsunami_prediction.ipynb

## Reports

- reports/datathon_tsunami_prediction.pdf

## Submissions

- submissions/submission_Nov23.csv

## License

See LICENSE