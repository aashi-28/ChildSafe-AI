<div align="center">

# 🛡️ ChildSafe AI

### AI-Powered Cyber Threat Detection Platform for Children's Online Safety

<p>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
<img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white"/>
<img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white"/>
<img src="https://img.shields.io/badge/Tesseract-OCR-blue?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Machine-Learning-success?style=for-the-badge"/>
<img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge"/>
</p>

<p>
<img src="https://img.shields.io/github/stars/aashi-28/ChildSafe-AI?style=flat-square"/>
<img src="https://img.shields.io/github/last-commit/aashi-28/ChildSafe-AI?style=flat-square"/>
<img src="https://img.shields.io/github/issues/aashi-28/ChildSafe-AI?style=flat-square"/>
</p>

**Detecting Cyberbullying • Phishing • Online Grooming • Blackmail using Machine Learning, NLP & OCR**

[Overview](#-overview) • [Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Demo](#-demo) • [Contributing](#-contributing)

</div>

---

## 📖 Overview

ChildSafe AI is an intelligent cyber threat detection platform designed to identify harmful online conversations involving children.

The application analyzes both **text messages** and **chat screenshots** to detect cyber threats including **cyberbullying, online grooming, phishing, and blackmail.**

By combining **Machine Learning**, **Natural Language Processing (NLP)**, and **Optical Character Recognition (OCR)**, ChildSafe AI helps parents, guardians, educators, and platform moderators quickly flag risky conversations through an interactive Streamlit web application.

> ⚠️ **Note:** This tool is intended to assist human judgment, not replace it. Always have a trusted adult review flagged conversations before taking action.

---

## ✨ Features

| Feature | Description |
|---|---|
| 💬 Cyberbullying Detection | Flags hostile, threatening, or demeaning language |
| 🎣 Phishing Detection | Identifies scam links, fake offers, and credential-harvesting attempts |
| 👤 Online Grooming Detection | Detects manipulative or predatory conversation patterns |
| ⚠️ Blackmail Detection | Flags coercive or extortion-style messages |
| 🖼️ OCR Screenshot Analysis | Extracts and analyzes text directly from chat screenshots |
| 🤖 ML Threat Prediction | Classifies threats using trained supervised models |
| 📊 Risk Level Assessment | Assigns a risk score/severity to each analyzed conversation |
| ☎️ Phone Number Extraction | Detects and validates phone numbers shared in conversations |
| 🌐 Interactive Dashboard | Clean, simple Streamlit interface for non-technical users |
| 📈 Model Comparison | Benchmarks multiple ML models side by side |

---

## 🏗️ System Architecture

```
                         User Input
                             │
              ┌──────────────┴──────────────┐
              │                             │
          Text Input                  Screenshot Upload
              │                             │
              │                       Tesseract OCR
              │                             │
              └──────────────┬──────────────┘
                             │
                    Text Preprocessing
                             │
              TF-IDF / CountVectorizer
                             │
       ┌─────────────────────┼─────────────────────┐
       │                     │                     │
 Logistic Regression   Decision Tree         Random Forest
       │                     │                     │
       └─────────────────────┼─────────────────────┘
                             │
                  Threat Classification
                             │
                  Risk Level Prediction
                             │
                Streamlit Web Interface
```

---

## ⚙️ Workflow

1. **Input** — User submits raw text or uploads a chat screenshot
2. **OCR Extraction** — If an image is provided, Tesseract OCR extracts the text
3. **Preprocessing** — Text is cleaned, normalized, and tokenized
4. **Feature Extraction** — TF-IDF / CountVectorizer converts text into numerical features
5. **Prediction** — Trained ML models classify the conversation
6. **Risk Scoring** — A severity/risk score is generated based on the prediction confidence
7. **Output** — Results are displayed on the Streamlit dashboard with an explanation

---

## 🧠 Machine Learning Models

The project compares multiple supervised learning algorithms for cyber threat detection.

| Model | Purpose |
|--------|----------|
| Logistic Regression | Baseline text classification |
| Decision Tree | Rule-based classification |
| Random Forest | Ensemble classification for improved accuracy |

Text features are extracted using:
- **TF-IDF Vectorizer**
- **Count Vectorizer**

---

## 💻 Tech Stack

| Category | Technologies |
|-----------|-------------|
| Programming Language | Python |
| Machine Learning | Scikit-learn |
| NLP | TF-IDF, CountVectorizer |
| OCR | Tesseract OCR |
| Frontend | Streamlit |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib |
| Version Control | Git & GitHub |

---

## 📂 Project Structure

```
ChildSafe-AI/
│
├── app.py               # Main Streamlit application
├── README.md
├── LICENSE
├── requirements.txt
│
├── data/                # Training/evaluation datasets
├── models/              # Saved/trained ML models
├── utils/               # Helper functions (OCR, preprocessing, etc.)
└── screenshots/          # App screenshots & demo GIF for this README
```

---

## 🚀 Installation

**1. Clone the repository**
```bash
git clone https://github.com/aashi-28/ChildSafe-AI.git
```

**2. Move into the project directory**
```bash
cd ChildSafe-AI
```

**3. (Optional) Create a virtual environment**
```bash
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
```

**4. Install dependencies**
```bash
pip install -r requirements.txt
```

> 🔧 **Tesseract OCR** must also be installed separately on your system:
> - **Windows:** [Download installer](https://github.com/UB-Mannheim/tesseract/wiki)
> - **macOS:** `brew install tesseract`
> - **Linux:** `sudo apt install tesseract-ocr`

**5. Run the application**
```bash
streamlit run app.py
```

The app will open automatically at `http://localhost:8501`.

---

## 🖥️ Usage

1. Launch the app with `streamlit run app.py`
2. Choose an input mode: **Text Analysis** or **Screenshot Analysis**
3. Paste a conversation or upload a chat screenshot
4. Click **Analyze**
5. Review the predicted threat category and risk level in the results panel

---

## 📸 Screenshots

> 📁 Add your images to the `screenshots/` folder using the filenames below, then they'll render automatically here.

| | |
|---|---|
| **Home Page** <br> `screenshots/home.png` | **Text Analysis** <br> `screenshots/text-analysis.png` |
| ![Home](screenshots/home.png) | ![Text Analysis](screenshots/text-analysis.png) |
| **OCR Analysis** <br> `screenshots/ocr-analysis.png` | **Prediction Result** <br> `screenshots/result.png` |
| ![OCR Analysis](screenshots/ocr-analysis.png) | ![Result](screenshots/result.png) |

<details>
<summary>📝 Markdown reference (click to expand)</summary>

```markdown
![Home](screenshots/home.png)
![Text Analysis](screenshots/text-analysis.png)
![OCR Analysis](screenshots/ocr-analysis.png)
![Result](screenshots/result.png)
```

</details>

---

## 🎥 Demo

<p align="center">
<img src="screenshots/demo.gif" width="850" alt="ChildSafe AI demo showing text and screenshot analysis">
</p>

> 🎬 **To add your own demo:**
> 1. Record a short screen capture of the app in action (tools like [ScreenToGif](https://www.screentogif.com/) or [Kap](https://getkap.co/) work well)
> 2. Save it as `screenshots/demo.gif` (keep it under ~10MB for fast GitHub loading)
> 3. The embed above will render automatically once the file is in place

---

## 📊 Model Evaluation

The machine learning models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

Comparing multiple classifiers helps determine the most suitable model for each threat category.

---

## 📈 Results

- ✔ Successfully detects multiple categories of cyber threats
- ✔ Supports both text-based and screenshot-based analysis
- ✔ Integrates OCR and machine learning into a single platform
- ✔ Provides interpretable threat classification and risk assessment

---

## 🎯 Future Enhancements

- [ ] Deep learning models (LSTM / BERT)
- [ ] Explainable AI (XAI) for prediction transparency
- [ ] Multi-language support
- [ ] Real-time chat monitoring
- [ ] Cloud deployment
- [ ] Mobile application
- [ ] Advanced threat intelligence integration

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m "Add your feature"`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 👩‍💻 Author

**Aashi Singh**
B.Tech Information Technology, Manipal University Jaipur

📧 [aashisang55@gmail.com](mailto:aashisang55@gmail.com)
🔗 [GitHub](https://github.com/aashi-28)
🔗 [LinkedIn](https://www.linkedin.com/in/aashi-singh-553494330/)

---

<div align="center">

### ⭐ If you found this project helpful, please consider giving it a Star!

</div>
