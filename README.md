# Automated Risk-Scoring System for Financial Institutions

The practical part of the automated transaction risk assessment system was developed in the master’s thesis. Includes scenario-based synthetic data creation, data-quality checks, class-imbalance handling, ML model selection, training/retraining.

This repository contains the source code and experimental artefacts for the master's thesis **"Automated Risk-Scoring System for Financial Institutions"**.  
The system implements an end-to-end workflow for suspicious / high-risk transaction detection, starting from scenario-driven synthetic data creation and finishing with model explainability.

## 1. Overview

The pipeline follows these main stages (see thesis diagram):

1. Choosing a data synthesis method  
2. Building a scenario catalogue (FI guidelines, EU directives)  
3. Synthetic transaction generation  
4. Data-quality check
5. Model selection (AutoML and expert shortlisting)
6. Class-imbalance handling (SMOTE / ADASYN / ROSE)  
7. Training / retraining mode and threshold update  
8. Adaptivity check  

This repository provides code, sample configs and notebooks for each stage.

## 2. Repository structure

```text
/1_data_synthesis/          # data synthesis method, generators, scenario specs
/2_scenario_catalogue/      # scenarios from FI/EU rules
/3_data_quality/            # rule-based validation, feature profiling
/4_model_selection/         # AutoML runs, feature importance, shortlist
/5_class_balance/           # SMOTE/ADASYN/ROSE, class weights, focal loss
/6_training_adaptation/     # incremental vs full retraining, thresholds
/meeting minutes/           # meeting minutes with supervisor
/artefacts/                 # supporting materials (presentations, Gantt chart, conference materials, Zotero library)

The full project repository is available at - https://github.com/NataKrj/Automated-Risk-Scoring-System.