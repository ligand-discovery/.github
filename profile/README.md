## Welcome to Ligand Discovery 🎯

Welcome to the Ligand Discovery Project's main codebase. This project is led by [Georg Winter's lab](https://www.winter-lab.com/) at [CeMM](https://cemm.at) in Vienna.

Below, you will find links to the repositories associated with the various components of the project:

#### Data Analysis & Paper Figures
- [**primary-paper-figures**](https://github.com/ligand-discovery/primary-paper-figures): Executable notebooks to produce the main paper figures.
- [**interactome-signatures**](https://github.com/ligand-discovery/interactome-signatures): Executable notebooks for discovering interactome signatures from the primary screening data.

#### Model Training
- [**fragment-embedding**](https://github.com/ligand-discovery/fragment-embedding): Train and predict fully-functionalized fragment descriptors.
- [**mini-automl**](https://github.com/ligand-discovery/mini-automl): Train small machine learning models using TabPFN. Includes scripts for promiscuity models and interactome signature models.
- [**mini-xai**](https://github.com/ligand-discovery/mini-xai): Notebook for the Shapley value analysis.

#### Streamlit Apps
- [**interactions**](https://github.com/ligand-discovery/interactions): explore screening data as a standalone application.
- [**protein-profile-explorer**](https://github.com/ligand-discovery/protein-profile-explorer): Deploy the protein profile explorer (a.k.a. background checker).
- [**protein-set-enrichment-analysis**](https://github.com/ligand-discovery/protein-set-enrichment-analysis): Deploy the protein set enrichment analysis.
- [**fragment-predictor**](https://github.com/ligand-discovery/fragment-predictor): Deploy the fragment predictor based on promiscuity and interactome signature models.
- [**on-the-fly-modeling**](https://github.com/ligand-discovery/on-the-fly-modeling): Simple app for on-demand modeling.
