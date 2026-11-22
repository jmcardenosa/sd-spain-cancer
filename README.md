# Data-Driven Discovery of Lung Cancer-Related Subgroups Using Public Data from Spain

## Description
This repository contains the processed datasets, visualization code, and graphical results associated with the paper *"Data-Driven Discovery of Lung Cancer-Related Subgroups Using Public Data from Spain"*. 

The study applies Subgroup Discovery (SD) techniques to analyze demographic, environmental, lifestyle, and socioeconomic factors. The goal is to identify population-level risk profiles (subgroups) significantly associated with lung cancer mortality and incidence in Spain.

## Repository structure

The repository is organized into the following main folders:

*   **`datasets/`**: contains the datasets resulting from integrating and preprocessing twelve Spanish public data sources (SIEC, MITECO, AEMET, INE, etc.). Data has been aggregated at the temporal (annual) and spatial (autonomous community) levels. To maximize the use of available information, two versions are provided:
    *   `age_included/`: preserves full age-group disaggregation, covering the 2011-2023 period. It includes general cancer files (`all_cancer_es.csv`, `all_cancer_en.csv`) and lung cancer-specific files (`lung_cancer_es.csv`, `lung_cancer_en.csv`).
    *   `age_removed/`: omits the age variable to incorporate a broader set of variables associated with the total population, covering the 2016-2023 period (excluding 2017 due to a high proportion of missing values). It includes homologous files to the previous folder.
    *   `variables_description/`: contains data dictionaries (`english.csv` and `spanish.csv`) documenting the meaning and possible values of each variable present in the datasets.

*   **`code/`**: contains Jupyter notebooks (available in both English and Spanish) developed for the evaluation and visualization of the variables. These notebooks generate graphical representations that allow inspecting the relative contribution and consistency of each predictor variable within the discovered subgroups.

*   **`results/`**: Stores the plots generated from the code notebooks. These graphical representations facilitate the clinical and epidemiological interpretation of the subgroups associated with both lung cancer mortality and incidence.
