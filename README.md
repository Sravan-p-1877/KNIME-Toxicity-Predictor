# KNIME-Toxicity-Predictor
A low-code machine learning model built in KNIME to predict the clinical toxicity of biochemical compounds.
# Biochemical Toxicity Prediction with KNIME

This project is a proof-of-concept for a low-code machine learning model that predicts the clinical toxicity of chemical compounds based on their structure. The entire workflow was built using the KNIME Analytics Platform.

---

## 💡 Overview
The model takes a chemical's SMILES string as input, calculates its molecular fingerprint, and uses a trained Random Forest model to classify it as toxic or non-toxic. A key feature of this workflow is its use of the **SMOTE** technique to handle severe class imbalance in the source data.

---

## 📋 Workflow
The workflow is divided into two main parts: model training/evaluation and a separate branch for predicting new compounds.


*Insert your `workflow.png` here by dragging and dropping it into this text editor.*

---

## 📈 Results
The initial model performed poorly on the minority (toxic) class due to data imbalance. After applying SMOTE, the model's ability to correctly identify toxic compounds improved dramatically from **9% to 94%**.

**Final Confusion Matrix:**

*Insert your `results.png` here.*

---

## 🚀 How to Use
1.  Download and install the [KNIME Analytics Platform](https://www.knime.com/downloads).
2.  Install the required extensions (KNIME Python Integration, KNIME Chemistry Extensions).
3.  Download the `Biochemical_Toxicity_Model.knwf` file from this repository.
4.  In KNIME, go to **File** → **Import KNIME Workflow...** and select the downloaded file.
5.  The workflow is now ready to be explored and executed.
