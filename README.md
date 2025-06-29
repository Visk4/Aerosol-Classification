# Aerosol-Classification

# Overview

This project implements the aerosol classification methodology described in the paper "Aerosol classification by application of machine learning spectral clustering algorithm" by Shantikumar S. Ningombam et al. It uses a spectral clustering algorithm to classify aerosol types (dust, urban/industrial, biomass burning, and mixed aerosols) based on AERONET data from 150 sites across six continents (Africa, Asia, Australia, Europe, North, and South America) spanning 1993–2022. The program, named AerosolClassifier, processes aerosol optical parameters to identify dominant aerosol types and their spatial and temporal variations.

# Reference Paper





Title: Aerosol classification by application of machine learning spectral clustering algorithm



# Authors:





Shantikumar S. Ningombam (Conceptualization, Methodology, Writing – original draft, Data reduction, Figures & analysis)



E.J.L. Larson (Data reduction, Figures, Visualization, Editing)



G. Indira (Data reduction, Visualization and plotting)



B.L. Madhavan (Conceptualization & reviewing the manuscript)



Pradeep Khatri (Conceptualization, Plotting and reviewing the manuscript)



Source: Published in Journal of Aerosol Science (2023), available at ScienceDirect



Description: The paper utilizes a multivariate spectral clustering algorithm to classify aerosols using five optical parameters: fine-mode Aerosol Optical Depth (AOD_Fine-mode), Extinction Angstrom Exponent (EAE), Single Scattering Albedo (SSA), Absorption Angstrom Exponent (AAE), and Real Refractive Index (RRI). The study highlights regional aerosol characteristics, such as dust dominance in Africa and biomass burning in Australia during September–November.

# Dataset

The dataset is sourced from AERONET and includes quality-assured measurements from 150 sites globally (1993–2022). It is hosted on Google Drive:
Download Dataset

# Program Details





# Name: AerosolClassifier



Description: A Python-based implementation of the spectral clustering algorithm for aerosol classification, processing AERONET data to identify four primary aerosol types. The code handles data preprocessing (imputation, scaling), feature engineering, and clustering, optimized for memory efficiency as tested in Google Colab.



Key Features:





Processes five aerosol optical parameters (AOD_Fine-mode, EAE, SSA, AAE, RRI)



Implements spectral clustering with eigenvalue/eigenvector projection



Validates clusters against threshold-based classification (FMF, SSA)



Handles spatial (continental) and temporal (yearly, seasonal) variations



Includes visualization tools for cluster analysis and land use/land cover (LULC) integration

Installation





Clone the repository:

git clone https://github.com/Visk4/Aerosol-Classification.git



Install dependencies:

pip install -r requirements.txt



Ensure Python 3.8+ is installed.

Usage


https://drive.google.com/drive/folders/1mYKPLzXhJt0k7Yl5KcQHXy62UE-3cBr1?usp=drive_link

Download the AERONET dataset from the Google Drive link above.



Place the dataset in the data/ directory.



Run the main script:

python aerosol_classifier.py



Adjust configuration in config.py for custom parameters (e.g., clustering thresholds, sample size).

Requirements





Python 3.8+



Libraries: numpy, pandas, scikit-learn, matplotlib, seaborn (see requirements.txt)



Optional: Google Colab for large-scale data processing

Project Structure





aerosol_classifier.py: Main script for data processing and clustering



data/: Directory for AERONET dataset



config.py: Configuration file for clustering parameters



visualizations/: Scripts for generating plots (e.g., cluster scatter plots, LULC maps)

Contributing

Contributions are welcome! Please submit pull requests or open issues for bugs, feature requests, or improvements. Ensure code follows PEP 8 standards and includes documentation.

License

This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments





AERONET for providing the dataset



Authors of the referenced paper for their foundational work



Support from [your institution or funding source, if applicable]
