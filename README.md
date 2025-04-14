# Capstone-Project
# 🧠 Estimating the Risk of Depression among Dementia Caregivers

A machine learning and NLP-driven feasibility study aimed at early detection of depression and perceived burden in caregivers of people with dementia (PwD). This project demonstrates how informal caregiver narratives and demographic data can be transformed into predictive insights to support timely mental health intervention.

## 📌 Project Overview

Informal caregivers of PwD often face significant emotional and physical stress, which frequently goes unrecognized. This project explores whether it's possible to **predict the risk of depression and care burden** using a combination of:

- Demographic attributes (e.g., age, employment, relationship to care recipient)
- Narrative responses from semi-structured interviews

Using both structured and unstructured data, we trained and evaluated machine learning models to identify caregivers at risk.

## 📊 Key Results

- Achieved **F1 score of 0.72** for depression risk classification using narrative-based NLP features (SVM + Adjective-Containing Sentence model)
- Achieved **F1 score of 0.76** for caregiver burden prediction using demographic data (SVM model)
- Built over **2,800 NLP features** from caregiver interview transcripts using spaCy for preprocessing and feature extraction

## 🧰 Tools & Technologies

- **Languages**: Python
- **Libraries**: scikit-learn, spaCy, NumPy, pandas
- **NLP Techniques**: Bag-of-Words, adjective frequency analysis, feature engineering
- **Data**: Survey + Zoom interviews from 65 caregivers (transcribed and anonymized)
- **Modeling**: Logistic Regression, K-Nearest Neighbors, Support Vector Machines
- **Evaluation**: Leave-One-Subject-Out Cross-Validation (LOSO-CV), F1 score, confusion matrices

## 🧪 Methodology

1. **Data Collection**: Demographics + PHQ-8 and ZBI scores + open-ended interviews
2. **Feature Engineering**:
   - Demographic features one-hot encoded
   - NLP features extracted from adjective-heavy sentences
3. **Modeling**:
   - Trained separate models for depression and burden classification
   - Compared 7 feature sets × 3 algorithms (total 42 models)
4. **Evaluation**:
   - Selected best model for each task based on F1 scores and confusion matrix performance

## 📈 Impact

This project supports **early mental health screening in non-clinical settings** by leveraging everyday conversations. The approach can help social workers and care facilities flag at-risk individuals and intervene sooner—improving both caregiver well-being and patient outcomes.

## 🧬 Authors

- Kruthika Gaddam (Indiana University, Health Informatics)
- Mahesh Moodukonaje (Purdue University)
- Hyeju Jang, Hee-Tae Jung (Indiana University)

## 📄 Citation

If you use this project or build on our work, please cite our IEEE BHI 2024 paper

