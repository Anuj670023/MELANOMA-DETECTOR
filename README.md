# MELANOMA-DETECTOR 🩺

A deep learning model that classifies skin lesions as **Benign** or **Malignant Melanoma** using a CNN trained on dermatoscopic images.

## 📌 Kaggle Model Link
The pre-trained model weights and architecture are available on Kaggle:  
🔗 [https://www.kaggle.com/models/azure07i13/melanoma-detector](https://www.kaggle.com/models/azure07i13/melanoma-detector)

---

## 🛠 Setup & Installation

### 1. Clone the Repository
```bash
git clone https://github.com/Anuj670023/melanoma-classifier.git
cd melanoma-classifier
```

### 2. Download Model Files from Kaggle
You need the following files from Kaggle (place them in the project root):
- `Melanoma.h5` (Trained weights)

#### Using Kaggle API:
```bash
pip install kaggle
kaggle models download -u azure07i13 -m melanoma-detector
unzip melanoma-detector.zip
```

## 🚀 Running the App
```bash
streamlit run Melanoma_App.py
```

The app will launch in your browser at `http://localhost:8501`.

---

## 📂 File Structure
```
melanoma-classifier/
├── Melanoma_App.py       # Streamlit web interface
├── model_run.py          # CNN prediction logic
├── Melanoma.json         # Model architecture (from Kaggle)
├── Melanoma.h5           # Model weights (from Kaggle)
└── README.md
```

## 📋 Requirements
Create `requirements.txt` with:
```text
tensorflow==2.12.0
streamlit==1.28.0
opencv-python==4.8.0
numpy==1.24.0
pillow==10.0.0
kaggle==1.5.16
```

