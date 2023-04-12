## Welcome to Ligand Discovery 🎯

Welcome to the Ligand Discovery Project's main codebase. This project is led by [Georg Winter's lab](https://www.winter-lab.com/) at [CeMM](https://cemm.at) in Vienna. If you want to interact with our tools as a user, we recommend that you visit [https://ligand-discovery.ai](https://ligand-discovery.ai).

Below, you will find links to the repositories associated with the various components of the project:

#### Data Analysis & Paper Figures
- [**primary-paper-figures**](https://github.com/ligand-discovery/primary-paper-figures): Here you can find executable notebooks to produce the main paper figures.
- [**interactome-signatures**](https://github.com/ligand-discovery/interactome-signatures): This repository contains executable notebooks to discover interactome signatures from the primary screening data.

#### Model Training & Interpretability
- [**mini-automl**](https://github.com/ligand-discovery/mini-automl): Here you can find the code to train small machine learning models using TabPFN. Executable scripts are available for promiscuity models and interactome signature models.
- [**mini-xai**](https://github.com/ligand-discovery/mini-xai): Code in this repository is used to derive the interpretability tiles used for the promiscuity models.
- [**fragment-embedding**](https://github.com/ligand-discovery/fragment-embedding): This repository is used to train and predict fully-functionalized fragment descriptors.

#### Streamlit Apps
- [**fragment-predictor**](https://github.com/ligand-discovery/fragment-predictor): This repository contains the Streamlit App to deploy the fragment predictor, based on promiscuity and interactome signature models.
- [**protein-profile-explorer**](https://github.com/ligand-discovery/protein-profile-explorer): This repository contains the Streamlit App to deploy the protein profile explorer (a.k.a. background checker).
- [**protein-set-enrichment-analysis**](https://github.com/ligand-discovery/protein-set-enrichment-analysis): Here you can find the code to deploy the protein set enrichment analysis as a Streamlit App.
