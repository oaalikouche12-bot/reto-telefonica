# reto-telefonica

Academic project developed for the **Artificial Intelligence Challenge** course of the **MSc in Data Analytics for Business**.

This project focuses on **fake voice detection using machine learning**, with the goal of distinguishing between:

- **bonafide**: real audio
- **spoof**: fake or manipulated audio

The work is based on an end-to-end pipeline that transforms raw audio into numerical features, trains classification models, and evaluates their performance on a development set.

---

## Project overview

The main objective of this project is to build a baseline system for **audio anti-spoofing** using classical machine learning methods.

The workflow includes:

1. Loading and organizing the audio dataset
2. Reading official protocol files for labeling
3. Extracting acoustic features from audio signals
4. Transforming audio into tabular data
5. Training and comparing machine learning models
6. Evaluating results using classification metrics and learning curves

---

## Technologies used

- Python
- Google Colab / Jupyter Notebook
- pandas
- numpy
- librosa
- scikit-learn
- matplotlib

---

## Methodology

The project follows these main steps:

### 1. Data preparation
- Load audio files and metadata
- Use protocol files to assign labels
- Build structured datasets for training and development

### 2. Feature extraction
Acoustic features are extracted from each audio sample, including:
- duration
- amplitude statistics
- zero crossing rate
- RMS energy
- spectral centroid
- spectral bandwidth
- spectral rolloff
- MFCCs

### 3. Model training
Several supervised machine learning models are trained and compared, including:
- Random Forest
- HistGradientBoosting
- SVM
- Logistic Regression
- KNN

### 4. Evaluation
Model performance is assessed on the development set using:
- accuracy
- precision
- recall
- F1-score
- confusion matrix
- cross-validation
- learning curves

---

## Main results

The initial **Random Forest baseline** achieved:

- **Accuracy on dev set:** 0.87

After comparing different models, the best results obtained were:

- **Random Forest**: accuracy_dev = **0.893**
- **HistGradientBoosting**: accuracy_dev = **0.883**
- **SVM**: accuracy_dev = **0.876**
- **Logistic Regression**: accuracy_dev = **0.858**
- **KNN**: accuracy_dev = **0.819**

The best-performing model was **Random Forest**, showing solid and balanced performance for this baseline approach.

Learning curve analysis also showed that validation performance improves as the number of training examples increases, suggesting reasonable generalization and room for further improvement.

---

## Skills demonstrated

This project showcases practical skills in:

- data analysis
- feature engineering
- supervised machine learning
- model comparison
- metric interpretation
- end-to-end project development in notebooks

---

## Repository contents

- `Reto_Telefonica.ipynb`: main notebook containing the full workflow
- `README.md`: project description

---

## Notes

This is an **academic project** developed as part of a master's course.  
Its purpose is to apply machine learning techniques to a realistic AI problem related to **voice spoofing detection**.

---

## Author

**Omar Aalikouche**
