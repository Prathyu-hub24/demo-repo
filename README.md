# 🩺 Diabetes Prediction System (Gradio + Random Forest)

An **interactive AI-powered web application** that predicts whether a patient has diabetes based on medical attributes.
The system uses a **Random Forest classifier** trained on the **PIMA Indians Diabetes dataset** and provides predictions through a **modern Gradio (v6.3.0) UI**.

---

## 🚀 Features

* 🔍 **Diabetes prediction** using a trained Random Forest model
* 🎛️ **Interactive UI** with sliders and grouped inputs
* 📊 **Risk probability (%)** displayed with prediction
* 🟢 / 🔴 **Color-coded results** for better interpretability
* 🧠 Handles **missing values** using mean imputation
* ⚡ Ready for demos, portfolios, and interviews

---

## 🧪 Model Overview

* **Algorithm**: Random Forest Classifier
* **Preprocessing**:

  * Zero values treated as missing
  * Mean imputation using `SimpleImputer`
* **Train/Test Split**: 70% / 30%
* **Evaluation Metric**: Accuracy
* **Inference**: Real-time via Gradio UI

---

## 📂 Project Structure

```
├── app.py                  # Main Gradio application
├── pima-data.csv           # Dataset
├── README.md               # Project documentation
```

---

## 📥 Input Features

The model expects the following **8 medical inputs**:

| Feature      | Description                  |
| ------------ | ---------------------------- |
| num_preg     | Number of pregnancies        |
| glucose_conc | Plasma glucose concentration |
| diastolic_bp | Diastolic blood pressure     |
| insulin      | Serum insulin                |
| bmi          | Body Mass Index              |
| diab_pred    | Diabetes pedigree function   |
| age          | Age of the patient           |
| skin         | Skin thickness               |

---

## 📤 Output

* **Prediction**:

  * 🟥 HAS DIABETES
  * 🟩 NO DIABETES

* **Risk Probability**:

  * Likelihood of diabetes in percentage (%)

---

## 🛠️ Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/diabetes-prediction-gradio.git
cd diabetes-prediction-gradio
```

### 2️⃣ Install Dependencies

```bash
pip install gradio==6.3.0 scikit-learn pandas numpy matplotlib seaborn
```

---

## ▶️ Run the Application

```bash
python app.py
```

After running, open the **local Gradio URL** shown in the terminal (usually `http://127.0.0.1:7860`).

---

## 🧑‍⚕️ How to Use the UI

1. Enter patient details using sliders
2. Click **“Predict Diabetes Risk”**
3. View:

   * Diagnosis result
   * Probability score
4. Use **Reset** to clear results

---

## 📊 Sample Prediction

**Input**

```
Pregnancies: 3
Glucose: 120
BMI: 28.5
Age: 35
```

**Output**

```
🟩 NO DIABETES
🟢 Risk Probability: 22.45%
---

## 🌟 Future Enhancements

* SHAP-based explainability
* Model persistence (`joblib`)
* Hugging Face deployment
* REST API using FastAPI
* Confidence gauge visualization

---

## 👨‍💻 Author

**Prathyusha**
AI / ML Engineer
Python • Machine Learning • GenAI • Gradio • Scikit-learn

---


Just tell me 👍

