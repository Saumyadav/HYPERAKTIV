## Multimodal Passive Digital Biomarkers for ADHD Classification and Subtype Discovery

## Overview

This project implements a machine learning pipeline to detect ADHD symptoms in children using passive multimodal wearable sensor data. The approach combines heart rate variability metrics and physical activity patterns collected from wearable devices to distinguish between ADHD and non-ADHD individuals. The complete implementation is provided in the [final_submission.ipynb](final_submission.ipynb) notebook.

This implementation is based on our research paper: [Multimodal Passive Digital Biomarkers for ADHD Classification and Subtype Discovery](https://www.techrxiv.org/users/985420/articles/1361783-multimodal-passive-digital-biomarkers-for-adhd-classification-and-subtype-discovery?commit=d88e3bb9b34eebdc308722b709d63f89c639fd36)

## Motivation

Traditional ADHD diagnosis relies heavily on subjective behavioral assessments and questionnaires, which can be time-consuming and prone to bias. This project explores an objective, data-driven approach using wearable sensor technology to identify physiological and behavioral patterns associated with ADHD. By analyzing continuous monitoring data from daily activities, we aim to provide complementary insights that could support clinical diagnosis and monitoring.

## Dataset

The dataset consists of longitudinal wearable sensor data collected from children over multiple days:

- **HRV Data**: Heart rate variability measurements including inter-beat intervals (IBI) and beats per minute (BPM)
- **Activity Data**: Physical activity levels measured through accelerometry
- **Patient Information**: Clinical ADHD diagnosis labels and demographic information

Data is organized by patient ID with temporal alignment across modalities.

**Dataset Source**: The data used in this project is available at [OSF Storage](https://osf.io/3agwr/files/osfstorage)



## Technical Requirements

All required packages are listed in [requirements.txt](requirements.txt). Key dependencies include:

- pandas, numpy: Data manipulation
- scikit-learn: Machine learning algorithms
- hrvanalysis: HRV preprocessing and feature extraction
- tsfresh: Time-series feature extraction
- matplotlib, seaborn: Visualization
- imblearn: SMOTE for handling imbalanced data


## Project Structure

```
.
├── final_submission.ipynb     # Main analysis notebook
├── README.md                  # This file
├── requirements.txt           # Python dependencies
├── patient_info.csv          # Patient metadata and labels
└── dataset/                  # Raw sensor data files
    ├── activity_data/       # Accelerometry measurements
    └── hrv_data/            # Heart rate variability data
```

## References

### Research Paper

This implementation is based on our research paper:

**Multimodal Passive Digital Biomarkers for ADHD Classification and Subtype Discovery**

Paper Link: https://www.techrxiv.org/users/985420/articles/1361783-multimodal-passive-digital-biomarkers-for-adhd-classification-and-subtype-discovery?commit=d88e3bb9b34eebdc308722b709d63f89c639fd36


### Dataset

Dataset Link: https://osf.io/3agwr/files/osfstorage



## Usage

To reproduce the analysis:

1. Install dependencies: `pip install -r requirements.txt`
2. Ensure data files are in the correct directory structure
3. Open and run [final_submission.ipynb](final_submission.ipynb) sequentially
4. Results including models, plots, and metrics will be generated

## Citation

If you use this work, please cite:

```bibtex
@article{yadav2025multimodal,
  title={Multimodal Passive Digital Biomarkers for ADHD Classification and Subtype Discovery},
  author={Yadav, Saumya and Upadhyay, Aditya and Shukla, Jainendra},
  journal={Authorea Preprints},
  year={2025},
  publisher={Authorea}
}
```

## License

This project is for research and educational purposes.
