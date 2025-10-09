# 🩺 Disease Prediction System

A machine learning-powered web app for predicting diseases from symptoms, with explainable results and prescription suggestions. Built for rapid prototyping, research, and real-world deployment using Streamlit.

---

## 🚀 Features
- 🤖 Predicts diseases based on user-input symptoms
- 🧠 Uses Random Forest, SVM, and Naive Bayes models (ensemble)
- 📝 NLP preprocessing for robust symptom matching
- 📊 Model evaluation and performance metrics
- 💊 Prescription recommendations for predicted diseases
- 📈 Jupyter notebook for exploration and demo
- 🖼️ Modern, interactive UI with Streamlit

---

## 🌳 Project Structure

```text
Disease-Prediction-AI/
│
├── .gitignore            # Git ignore rules
├── LICENSE               # MIT License
├── pyproject.toml        # Python project config (optional)
├── README.md             # Project documentation
├── requirements.txt      # Python dependencies for pip
│
├── assets/               # Images, icons, and static assets
│   └── generated-icon.png
|   └── 1.png
|   └── 2.png
│
├── data/                 # Datasets
│   ├── Testing.csv
│   └── Training.csv
│
├── models/               # Trained model binaries
│   ├── nb_model.pkl
│   ├── rf_model.pkl
│   └── svm_model.pkl
│
├── notebooks/            # Jupyter notebooks for demo/experiments
│   └── disease_pred.ipynb
│
├── scripts/              # Utility scripts (training, evaluation)
│   ├── evaluate_model.py
│   └── train_models.py
│
└── src/                  # All source code
    ├── app.py                # Streamlit web app entry point
    ├── disease_pred.py       # Core logic for disease prediction (chat/CLI)
    ├── model.py              # DiseasePredictor class and ML logic
    ├── nlp_processor.py      # NLP utilities for symptom extraction
    ├── prescriptions.py      # Maps diseases to prescription recommendations
    └── symptoms.py           # Loads available symptoms from training data
```

---
## Live Demo on Streamlit

[Demo](https://disease-prediction-ai-demo.streamlit.app/)
--

## Screenshots

## **UI 1**
![UI 1](https://github.com/mahlakechris93/Disease-Prediction-AI/blob/main/assets/1.png)

### **UI 2**
![UI 2](https://github.com/mahlakechris93/Disease-Prediction-AI/blob/main/assets/2.png)

   
## ⚙️ Setup

1. **Clone the repository**
   ```bash
   git clone <repo-url>
   cd Disease-Prediction-AI
   ```
2. **Create and activate a virtual environment**
   ```bash
   python -m venv venv
   # On Windows:
   venv\Scripts\activate
   # On Mac/Linux:
   source venv/bin/activate
   ```
3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

---

## 🖥️ Usage

### 🌐 Run the Streamlit Web App
```bash
streamlit run app.py
```
- Open the provided local URL in your browser.
- Enter your symptoms in the chat to get predictions and recommendations.

### 🧪 Retrain Models (Optional)
```bash
python train_models.py
```
- This will retrain and overwrite the `.pkl` model files using `Training.csv`.

### 📊 Evaluate Models (Optional)
```bash
python evaluate_model.py
```
- Outputs accuracy and confusion matrix for the current models.

### 📓 Explore in Jupyter Notebook
```bash
jupyter notebook disease_pred.ipynb
```

---

## 🙋 Author

Developed by **Chris Mahlake**


[![GitHub](https://img.shields.io/badge/-GitHub-181717?style=flat&logo=github&logoColor=white)](https://github.com/mahlakechris93)&nbsp;&nbsp;[![Email](https://img.shields.io/badge/-Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:mahlakechris93@gmail.com)&nbsp;&nbsp;[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/chris-mahlake-623428213/)


---


## 📄 License

This project is licensed under the MIT License.
