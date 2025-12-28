# Nanoparticle Toxicity Predictor

**Source:** [Kaggle - Nanoparticle Toxicity Dataset](https://www.kaggle.com/datasets/ucimachinelearning/nanoparticle-toxicity-dataset).

## Project Overview

The primary objective of this project is to develop and evaluate machine learning models capable of predicting the **toxicity outcome** (Toxic vs. nonToxic) of various nanoparticles (NPs). Using a dataset of 881 entries, the model analyzes physical and chemical parameters to identify safety risks associated with specific nanomaterials.

## Dataset & Variables

The analysis focuses on 11 key variables derived from a broader set of 19 parameters.

* **Target Variable:** `class` (0 = nonToxic, 1 = Toxic).
* **Nanoparticles Studied:** Aluminum Oxide (Al2O3), Copper Oxide (CuO), Iron Oxide (Fe2O3), Titanium Dioxide (TiO2), and Zinc Oxide (ZnO).
* **Key Features:**
* **Coresize:** Inner diameter of the nanoparticle.
* **Hydrosize:** Hydrodynamic size.
* **Surfcharge & Surfarea:** Surface charge and surface area.
* **Dosage & Expotime:** Concentration used and duration of exposure.
* **NOxygen:** Number of oxygen atoms in the NP.


## Methodology & Workflow

1. **Data Preprocessing:** Categorical labels for both the nanoparticle types and toxicity classes were numerically mapped (e.g., Al2O3 → 1, Toxic → 1).
2. **Exploratory Data Analysis (EDA):** Performed descriptive statistics, correlation analysis, and data visualization using `Seaborn` and `Matplotlib` to understand feature relationships.
3. **Model Selection:** Evaluated multiple classification algorithms:
* Decision Tree (Base and Tuned)
* Random Forest
* Bagging Classifier (Base and Tuned)


4. **Evaluation:** Models were compared and ranked based on their **Test F1 Score** to ensure a balance between precision and recall, note recall should be prioritized for this health use case.

## Results

The project provides a comprehensive comparison frame tracking **Accuracy, Recall, Precision, and F1 Scores** for both training and testing phases across all implemented models, with accuracy up to 97%.

* **Languages:** Python
* **Libraries:** Pandas, NumPy, Scikit-learn, Scipy, Seaborn, Matplotlib
