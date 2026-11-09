# Handwriting Classification

![Python](https://img.shields.io/badge/python-3.14-blue)

Proyek ini mengekstrak fitur tekstur tulisan tangan menggunakan GLCM, lalu menggunakannya untuk melatih model klasifikasi.

## Features
- Ekstraksi fitur GLCM dari gambar di folder `datasets/`.
- Pencarian parameter dan klasifikasi menggunakan SVM, XGBoost, dan LightGBM.

## Tech Stack
Python, scikit-image, OpenCV, scikit-learn, XGBoost, LightGBM, pandas

## Getting Started

### Prerequisites
- Python 3.14
- VS Code dengan ekstensi Jupyter, atau editor notebook lain

### Installation
```bash
git clone https://github.com/YosiaCoKR/handwriting-classification.git
cd handwriting-classification
python -m venv .venv
```

Aktifkan environment, lalu pasang dependensi:

```bash
# Linux/macOS
source .venv/bin/activate

# Windows PowerShell
.\.venv\Scripts\Activate.ps1

python -m pip install -r requirements.txt
```

### Usage
1. Buka `code.ipynb` dan pilih kernel dari environment `.venv`.
2. Jalankan cell notebook dari atas untuk mengekstrak fitur dan melatih model.

Notebook menyimpan hasil ekstraksi ke `glcm_features.csv`. Proses pencarian parameter model dapat memerlukan waktu.

## Project Structure
```text
.
├── code.ipynb
├── datasets/
│   ├── Eric/
│   ├── Felix/
│   └── Yosia/
├── glcm_features.csv
└── requirements.txt
```
