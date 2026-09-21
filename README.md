# Triple-Negative Breast Cancer: Diagnosis and Prognosis with Advanced Machine Learning

Detection and prognostic modelling for triple-negative breast cancer (TNBC). The work combines YOLO-based detection on breast cancer imaging with shrinkage operators, sequence networks, Kamada-Kawai graph layouts and elbow-method cluster analysis, followed by a clinical validation phase on hospital cohort data.

This repository is part of a wider cancer imaging and medical imaging portfolio; see the [profile overview](https://github.com/datascintist-abusufian) for related work in dermoscopy, brain MRI and lung adenocarcinoma.

## Contents

### Detection on imaging data

- `Yolov_model_demonstration_sufi.ipynb` — YOLO detection model demonstration.
- `Yolo_Model_Result_Visualisation_sufi.ipynb` — visualisation and inspection of detection outputs.

### Modelling and prognostic analysis

- `Breast cancer detection_python_demonstration_sufi.ipynb` — baseline detection workflow.
- `Breast__Cancer_Detection__by_advanced_machine_learning_sufi_13_12_2023_.ipynb` — advanced machine learning pipeline.
- `Breast_Cancer_updated_code_new (1).ipynb` — revised pipeline.
- `phase_analysis_26_02_2024.ipynb` — phase analysis.
- `Supplimentary_phase_26-02-2024.ipynb` — supplementary analyses.

### Clinical validation

- `Clinical_Hospital_Data_Xian_Jiaotong_University_.ipynb` — analysis of the hospital cohort.
- `Clinical_Hospital_Data_Xian_Jiaotong_University_Validation_.ipynb` — validation stage on the same cohort.
- `Clinical_validation_discovery phase.Rmd` — discovery-phase validation in R.
- `Hospital Trial_Data.csv` — trial dataset used by the validation notebooks.
- `Dataset Documentation of Breast Cancer detection_13-12-2023_sufi.pdf` — dataset documentation.

## Method summary

Detection is handled by YOLO-family models applied to breast cancer imaging. Feature selection uses shrinkage operators; sequence networks provide representation learning over the selected features; Kamada-Kawai graph layouts are used to inspect structure in the feature space; and the elbow method selects the number of clusters for prognostic grouping. Results move through a discovery phase and a separate validation phase on hospital cohort data rather than being reported on a single split.

## Running the notebooks

The notebooks run in Jupyter or Google Colab with a standard Python data-science stack (NumPy, pandas, scikit-learn, matplotlib) plus PyTorch and the Ultralytics YOLO package for the detection notebooks. The R Markdown file requires R with the packages loaded at the top of the document. Open a notebook and run cells in order; paths to `Hospital Trial_Data.csv` are relative to the repository root.

## Data

The hospital cohort notebooks reference clinical trial data associated with Xi'an Jiaotong University. See the dataset documentation PDF in this repository for the description of variables and collection. Imaging datasets used for detection are not redistributed here.

## Disclaimer

Research and educational use only. This is not a medical device and must not be used for clinical diagnosis or treatment decisions.

## Author

Md Abu Sufian — PhD researcher, University of East London. [GitHub](https://github.com/datascintist-abusufian) · [Google Scholar](https://scholar.google.com/citations?user=8ozStcUAAAAJ&hl=en)
