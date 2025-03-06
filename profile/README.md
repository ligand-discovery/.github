## Welcome to Ligand Discovery 🎯

This project enables exploration of a large scale fragment-based chemoproteomics screening data.

- Browse web apps that we deployed in a cloud server (or)
- Run apps locally by forking the code from [GitHub](https://github.com/ligand-discovery) (or)
- Download [Screening](https://github.com/ligand-discovery/landing-page/raw/refs/heads/main/assets/screeningData.tar.xz) data and [Competition](https://github.com/ligand-discovery/landing-page/raw/refs/heads/main/assets/competitionData.tar.xz) data for your own research

:warning: web app will sleep if inactive for few days; if web app is inactive, a `Restart this Space` button will appear within the web app. Click that button to reload the app.

### 1. :dart: **Interactions** 

   |[Web App](https://1.ligand-discovery.ai)|[Code Repo](https://github.com/ligand-discovery/interactions)|[DOI](https://doi.org/10.5281/zenodo.14935845)
   |---|---|---|

Explore the interactions between ligands and proteins. This is the main navigator to the chemoproteomics data, containing profiles for 407 fragments. The app also showcases competition assays for a few selected fragments

### 2. :mag: **Explore protein sets**
   
   |[Web App](https://2.ligand-discovery.ai)|[Code Repo](https://github.com/ligand-discovery/protein-profile-explorer)|[DOI](https://zenodo.org/records/10838104)
   |---|---|---|

With this tool, you can in put a set of proteins and see how many fragments interact with them according to our chemoproteomics data. We categorize proteins by their promiscuity/specificity levels to easily detect reported effect such as labeling bias
   
### 3. :mountain: **Protein set enrichment analysis**

   |[Web App](https://3.ligand-discovery.ai)|[Code Repo](https://github.com/ligand-discovery/protein-set-enrichment-analysis)|[DOI](https://zenodo.org/records/10838110)
   |---|---|---|

Explore fragment profiles from an enrichment perspective. We capture protein annotations of multiple scopes, from domains and families to molecular functions and cellular localization. We offer global and detailed views for each fragment
   
### 4. :chart_with_upwards_trend: **Fragment predictor**
   
   |[Web App](https://4.ligand-discovery.ai)|[Code Repo](https://github.com/ligand-discovery/fragment-predictor)|[DOI](https://zenodo.org/records/10838071)
   |---|---|---|

Predict whether your fully-functionalized fragment of interest is likely to be promiscuous or associated with a specific interactome signature. We have predefined 10 interactome signatures capturing high-level biological processes that emerged from our chemoproteomics data
   
### 5. :rocket: **On-the-fly modeling**

   |[Web App](https://5.ligand-discovery.ai)|[Code Repo](https://github.com/ligand-discovery/on-the-fly-modeling)|[DOI](https://zenodo.org/records/10838098)
   |---|---|---|

Build a machine learning model on the fly to predict potential interactions between your fully-functionalized fragments and proteins of interest. Sets of proteins are accepted and organized in coherent subsets to maximize the chance of obtaining a good model

---

This project was led by [Georg Winter](https://www.winter-lab.com/)'s group at [CeMM](https://cemm.at)

Cite: [Offensperger et al., Science (2024)](https://doi.org/10.1126/science.adk5864) 

---

Additional code repositories associated with the project:

Data Analysis & Paper Figures
- [**primary-paper-figures**](https://github.com/ligand-discovery/primary-paper-figures): Executable notebooks to produce the main paper figures. [DOI](https://zenodo.org/records/10838149).
- [**interactome-signatures**](https://github.com/ligand-discovery/interactome-signatures): Executable notebooks for discovering interactome signatures from the primary screening data. [DOI](https://zenodo.org/records/10838089)

Model Training
- [**fragment-embedding**](https://github.com/ligand-discovery/fragment-embedding): Train and predict fully-functionalized fragment descriptors. [DOI](https://zenodo.org/records/10838065)
- [**mini-automl**](https://github.com/ligand-discovery/mini-automl): Train small machine learning models using TabPFN. Includes scripts for promiscuity models and interactome signature models. [DOI](https://zenodo.org/records/10838095)
- [**mini-xai**](https://github.com/ligand-discovery/mini-xai): Notebook for the Shapley value analysis. [DOI](https://zenodo.org/records/10838141)
