# School Attendance Data Analysis

## Project context

Developed during Western Governors University coursework. This repository is a record of my implementation and learning, not a client engagement, deployed operational system, or claim of a new algorithm. Supplied requirements, starter components, datasets, and third-party libraries are distinct from my own implementation. Where their exact provenance or redistribution terms have not been established, they are not represented as my original work or as cleared for public release.


A data-preparation and exploratory machine-learning project focused on multi-year public-school attendance data. The notebook cleans the dataset, normalizes numerical features, and explores its structure with unsupervised clustering.

## Data preparation

The workflow includes:

- Median imputation for missing numeric values
- Categorical imputation for sparse text fields
- Removal of aggregate rows that duplicate lower-level observations
- IQR-based outlier capping
- Standardization with `StandardScaler`
- Comparison of broader and attendance-focused feature sets

## Analysis

K-Means clustering is evaluated across multiple values of `k` using silhouette scores. The notebook compares clusters produced from the complete feature set with clusters based on attendance-rate features to illustrate how feature selection changes the resulting structure.

## Files

- `School_Attendance_Dataset_Analysis.ipynb` — end-to-end analysis notebook
- `School_Attendance_dataset.csv` — dataset used by the notebook

## Run

Open the notebook in JupyterLab, Jupyter Notebook, or a compatible notebook environment. Install the Python packages imported by the notebook before executing its cells.

## Topics demonstrated

Data cleaning, missing-value handling, outlier treatment, feature scaling, K-Means clustering, silhouette analysis, feature-selection reasoning, and exploratory model evaluation.

## Public portfolio release

This is a publication copy of my WGU coursework implementation and subsequent revisions. The original development history is retained privately. Assessment documents, student identifiers, and training-data snapshots are excluded from this public history. Notebook outputs are cleared; recorded evaluation artifacts are retained separately where available. The academic origin and third-party dependencies remain attributed.

The attendance CSV is not distributed. Supply an authorized local `School_Attendance_dataset.csv` with the expected schema to execute the historical notebook. No new evaluation is claimed.
