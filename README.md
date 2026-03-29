# Predictive-Healthcare-Analytics
Mining Unstructured Data Assessment Task 1 Implementation - Macquarie University 

README
Project: Unstructured Data Mining in IoT-Enabled Healthcare (Demo)
Purpose

The purpose of this project is to demonstrate a framework for mining structured and unstructured healthcare data in a hospital IoT context. The goal is to show how structured physiological data (vitals, lab results) and unstructured clinical notes can be preprocessed, combined, and used for predictive modeling to generate risk scores, alerts, and decision support insights. This project focuses on methodology and workflow design rather than full-scale implementation.

What I Did

Data Loading: Loaded structured hospital data (CHARTEVENTS, LABEVENTS, ADMISSIONS) and unstructured clinical notes (NOTEEVENTS) from CSV files.

Structured Data Preprocessing: Filled missing values, normalized numeric features, and aggregated measurements per hospital admission.

Unstructured Data Pipeline: Prepared clinical notes by cleaning, lowercasing, tokenizing, and tagging for future Doc2Vec embeddings. Training of embeddings was not performed in the demo.

Feature Fusion: Combined structured features with placeholder embeddings to create a multimodal feature matrix.

Demo Predictive Modeling: Trained a Random Forest model on a placeholder target to demonstrate the workflow and generated risk scores for each patient.

Visualization: Produced a top-10 feature importance plot and a demo risk dashboard showing predicted risk scores and labels.


Dataset

Demo Dataset: The project uses a subset of hospital IoT and clinical data stored as CSV files. 

It includes:

CHARTEVENTS.csv – sensor-based vitals

LABEVENTS.csv – lab test results

ADMISSIONS.csv – admission details and patient IDs

NOTEEVENTS.csv – unstructured clinical notes

Why a Demo: The full hospital dataset (e.g., MIMIC-III) contains sensitive patient information. The demo dataset simulates the structure and type of real data, enabling demonstration of methodology without accessing private records.



