<<<<<<< HEAD
# A Deep Learning Approach for Culture-Free Bacterial Meningitis Diagnosis and ICU Outcome Prediction

This repository contains the code and data processing scripts supporting the study described in our recently submitted manuscript. Our work focuses on accelerating the diagnosis of bacterial meningitis and improving survival predictions for patients admitted to the intensive care unit (ICU) with suspected neuroinfectious diseases. This framework leverages both structured and unstructured data extracted from the MIMIC database to build and validate predictive machine learning models.

## Project Overview

### Background  
Traditional cerebrospinal fluid (CSF) culture—an essential diagnostic tool for neuroinfectious diseases—faces sensitivity and timeliness challenges, especially in patients who have received antibiotics. Our study introduces a machine learning-based approach aimed at:  
1. **Aim 1:** Predicting bacterial meningitis (redefined from CSF culture outcomes for enhanced clinical relevance), thereby reducing dependence on time-consuming and sometimes unreliable culture results.  
2. **Aim 2:** Predicting patient outcomes (e.g., hospital mortality) using both structured and unstructured clinical data, evaluating the performance of unimodal (structured data only) vs. multimodal (structured + unstructured data) predictive models.

### Overall Code Structure  
This repository is organized into five main sections:

1. **Data Extraction:**  
   - Scripts for extracting structured and unstructured data from the MIMIC database.

2. **Data Preprocessing:**  
   - Procedures for handling missing values, outliers, and other data quality issues.  
   - Preprocessing steps for textual data as well as numeric features.

3. **Modeling & Validation for Aim 1:**  
   - Establishment and validation of the CSF culture-based model.  
   - Re-labeled “corrected CSF culture outcomes” model building and evaluation.  
   - Refer to our manuscript for the detailed theoretical basis and model design.

4. **Modeling & Validation for Aim 2:**  
   - Comparisons between models using only structured data and those integrating both structured and unstructured inputs.  
   - Includes code for training, tuning, and validating the corresponding models.

5. **Independent Validation & Evaluation:**  
   - Code for extracting independent validation sets.  
   - Final evaluation scripts for Aim 1 and Aim 2 models, ensuring robust and unbiased performance assessment.

## Usage and Dependencies

The code uses the following major Python packages (with versions):

- `huggingface-hub` 0.17.3  
- `keras` 2.10.0  
- `matplotlib` 3.5.1  
- `numpy` 1.22.4  
- `pandas` 1.3.5  
- `scipy` 1.7.3  
- `tensorflow-gpu` 2.10.0  
- `transformers` 4.35.0

For a complete list of all dependencies, please refer to the `installed_packages.xlsx` file included in this repository.

## Additional Information

- For more detailed descriptions of model architectures, methodological rationale, and data handling procedures, please consult our published SCI paper.
- Should you have any questions or need further clarification, feel free to leave a comment on this GitHub project’s issues page.

---

This README provides an organized and polished summary of the project’s objectives, data handling procedures, modeling strategies, and dependencies. It supplements our academic paper and serves as a guide to the code and analyses we performed.
=======
# CNS Model Code
1. In the procedure code, aim1 refers to the prediction of a positive or negative CSF bacterial culture; aim2 refers to the prediction of the patient's hospital outcome.
2. Drawing upon clinical practice, authoritative references, and ICD documentation, we have redefined the labeling of positive and negative CSF bacterial cultures to reflect whether a patient is diagnosed with bacterial meningitis. This newly established model possesses greater practical relevance and coherence.
3. For more details, please refer to our SCI paper
>>>>>>> dc58b050f8e4f95d2576849eba7b4f0d0af2c338
