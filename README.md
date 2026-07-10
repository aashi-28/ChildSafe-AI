<div align="center">

# 🛡️ ChildSafe AI
### AI-Powered Cyber Threat Detection for Children's Online Safety

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white)
![OCR](https://img.shields.io/badge/OCR-Tesseract-blue?style=flat)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-success?style=flat)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat)

**Detecting cyberbullying, phishing, online grooming, and malicious conversations using Machine Learning, NLP, and OCR.**

</div>

---

# 📖 About the Project

ChildSafe AI is an intelligent cyber threat detection system designed to identify harmful online conversations involving children.

The application analyzes both **text messages** and **chat screenshots** to detect cyber threats such as:

- Cyberbullying
- Online Grooming
- Phishing
- Blackmail
- Malicious Conversations

The project combines **Natural Language Processing (NLP)**, **Machine Learning**, and **Optical Character Recognition (OCR)** to classify conversations and estimate their threat level through an interactive Streamlit application.

---

# ✨ Features

- 💬 Detects cyberbullying, phishing, grooming, and blackmail messages
- 🖼️ OCR-based screenshot analysis using Tesseract OCR
- 🤖 Machine Learning-based threat prediction
- 📊 Multiple model comparison
- ⚠️ Risk level prediction
- 📱 Phone number extraction and validation
- 🌐 Interactive Streamlit dashboard
- 📈 Performance evaluation using confusion matrices

---

# 🧠 Machine Learning Models

The project trains and evaluates multiple classification models:

- Logistic Regression
- Decision Tree
- Random Forest

Different text vectorization techniques were used:

- TF-IDF Vectorizer
- Count Vectorizer

The best-performing model is used for prediction within the application.

---

# ⚙️ Tech Stack

| Category | Technologies |
|-----------|--------------|
| Language | Python |
| Machine Learning | Scikit-learn |
| NLP | TF-IDF, CountVectorizer |
| OCR | Tesseract OCR |
| Frontend | Streamlit |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib |

---

# 📂 Project Structure

```
ChildSafe-AI/
│
├── app.py
├── data/
├── models/
├── utils/
├── requirements.txt
├── README.md
└── .gitignore
```

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/aashi-28/ChildSafe-AI.git
```

Move into the project directory

```bash
cd ChildSafe-AI
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the Streamlit application

```bash
streamlit run app.py
```

---

# 📊 Workflow

```
User Input
      │
      ▼
Text / Screenshot
      │
      ▼
OCR (if image)
      │
      ▼
Text Preprocessing
      │
      ▼
Feature Extraction
(TF-IDF / Count Vectorizer)
      │
      ▼
Machine Learning Model
      │
      ▼
Threat Classification
      │
      ▼
Risk Level Prediction
```

---

# 📈 Model Evaluation

The models were evaluated using:

- Accuracy
- Confusion Matrix
- Classification Report

The application compares different Machine Learning algorithms to determine the most effective classifier for cyber threat detection.

---

# 📸 Screenshots

Add screenshots inside a folder named **screenshots** and update these image links.

```
screenshots/
│
├── home.png
├── text-analysis.png
├── image-analysis.png
└── result.png
```

Example

```markdown
![Home](screenshots/home.png)

![Result](screenshots/result.png)
```

---

# 🎯 Future Improvements

- Deep Learning (LSTM/BERT)
- Real-time chat monitoring
- Multi-language support
- Explainable AI
- Cloud deployment
- Mobile application

---

# 👩‍💻 Author

**Aashi Singh**

B.Tech Information Technology  
Manipal University Jaipur

GitHub:
https://github.com/aashi-28

LinkedIn:
https://www.linkedin.com/in/aashi-singh-553494330/

---

# 📄 License

This project is licensed under the MIT License.

See the [LICENSE](LICENSE) file for details.
