# Arabic Medical Semantic Qualifiers 💉

This repository contains the full implementation and documentation of our graduation project titled:

**"Arabic Medical Semantic Qualifiers for Symptom Extraction and Diagnosis Prediction"**  
Bachelor's degree in Computer Engineering – Birzeit University  
**Authors**: Hidaya Mustafa, Rana Odeh, Katya Kobari  
**Supervisor**: Dr. Adnan Yahya  
**In collaboration with**: Dr. Lujain Alsadder (Queen Mary University of London)  
📅 **Date**: July 2025

---

## 🧠 Project Overview

Arabic-speaking healthcare systems often suffer from a lack of structured, standardized tools for understanding symptom descriptions in patient-doctor dialogues. Our project addresses this gap by building a complete AI pipeline capable of:

- Extracting symptoms and semantic qualifiers (e.g., **time**, **location**, **severity**, **duration**, **spread**) from **Arabic medical dialogues**
- Mapping extracted expressions to **SNOMED CT medical concepts**
- Predicting the **most likely cardiac diagnosis** using a trained machine learning model
- Presenting results via a **bilingual web interface** (Arabic and English)

---

## 🔍 Key Features

### ✅ Data Collection
- Real-world Arabic medical dialogues from clinical sources
- AI-generated dialogues to simulate rare and diverse cases

### ⚙️ Preprocessing & Feature Engineering
- Tokenization using AraBERT tokenizer
- Stop word removal, normalization, and standardization
- Rule-based extraction of symptoms and qualifiers

### 🏷️ BIO Tagging & Sequence Labeling
- BIO format labeling for symptoms and qualifiers
- Model trained using **AraBERT + BiLSTM + CRF**

### 🧩 Diagnosis Classification
- Logistic Regression model fine-tuned on cardiac data
- Converts extracted symptoms into binary input vector
- Predicts likely heart condition and confidence score

### 🌐 Web Application
- Frontend: HTML, CSS, JavaScript (Arabic support)
- Backend: Flask (Python) for processing and AI integration
- Results displayed as structured bilingual medical analysis

---

## 📁 Project Structure

| File | Description |
|------|-------------|
| `Graduation_Project.ipynb` | Jupyter notebook with all AI and preprocessing steps |
| `Report.pdf` | Full academic report detailing system design, implementation, and results |
| `Presentation.pptx` | Final project presentation slides |
| `data/` | Input dialogues, web files, and outputs (we will add it soon) |

---

## 📊 Evaluation

The system was trained and evaluated on both **real** and **AI-generated Arabic medical dialogues**.

- For the **symptom and qualifier extraction task** (BIO tagging), the **AraBERT + BiLSTM + CRF** model achieved **95.09% token-level accuracy** on the **validation set of AI-generated data**.

- For the **diagnosis prediction task**, the **Logistic Regression** classifier reached **87.94% accuracy** on a **cardiac-specific dataset**, based on the presence or absence of extracted symptoms.
---

## 🔒 Limitations

- Limited availability of high-quality Arabic medical datasets
- Model performance may drop on extremely rare symptoms
- AI-generated dialogues may lack full real-world nuance

---

## 🔭 Future Work

- Expand diagnosis coverage beyond heart-related conditions
- Improve handling of colloquial Arabic and dialectal expressions
- Integrate the system into real clinical workflows or EHR systems

---

## 📬 Contact

For inquiries or collaboration:

- 📧 hidayamustafa3@gmail.com  
- 📧 katyakobari@gmail.com
- 📧 rodeh4165@gmail.com

---

## 📝 Citation

If you use this work or refer to it in your research, please cite:
Katya Kobari, Hidaya Mustafa, Rana Odeh. "Arabic Medical Semantic Qualifiers", Birzeit University, July 2025.
