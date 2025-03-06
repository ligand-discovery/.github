## Welcome to Ligand Discovery 🎯

This project enables exploration of a large scale fragment-based chemoproteomics screening data.

> [!Note]
> Browse web apps that we deployed in an external cloud server (or)
> Run apps locally by forking the code from [GitHub](https://github.com/ligand-discovery) (or)
> Download [Screening](https://github.com/ligand-discovery/landing-page/raw/refs/heads/main/assets/screeningData.tar.xz) data and [Competition](https://github.com/ligand-discovery/landing-page/raw/refs/heads/main/assets/competitionData.tar.xz) data for your own research

> [!Tip] 
> web app will sleep if inactive for few days :sleeping:; if a web app is inactive, a `Restart this Space` button will appear within the web app. Click that button to reload the app.

### 1. :dart: **Interactions** 

   |[Web App :arrow_upper_right:](https://1.ligand-discovery.ai)|[Code Repo](https://github.com/ligand-discovery/interactions)|[DOI](https://doi.org/10.5281/zenodo.14935845)
   |---|---|---|

Explore the interactions between ligands and proteins. This is the main navigator to the chemoproteomics data, containing profiles for 407 fragments. The app also showcases competition assays for a few selected fragments

### 2. :mag: **Explore protein sets**
   
   |[Web App](https://2.ligand-discovery.ai) :arrow_upper_right:|[Code Repo](https://github.com/ligand-discovery/protein-profile-explorer)|[DOI](https://zenodo.org/records/10838104)
   |---|---|---|

With this tool, you can in put a set of proteins and see how many fragments interact with them according to our chemoproteomics data. We categorize proteins by their promiscuity/specificity levels to easily detect reported effect such as labeling bias
   
### 3. :mountain: **Protein set enrichment analysis**

   |[Web App](https://3.ligand-discovery.ai) :arrow_upper_right:|[Code Repo](https://github.com/ligand-discovery/protein-set-enrichment-analysis)|[DOI](https://zenodo.org/records/10838110)
   |---|---|---|

Explore fragment profiles from an enrichment perspective. We capture protein annotations of multiple scopes, from domains and families to molecular functions and cellular localization. We offer global and detailed views for each fragment
   
### 4. :chart_with_upwards_trend: **Fragment predictor**
   
   |[Web App](https://4.ligand-discovery.ai) :arrow_upper_right:|[Code Repo](https://github.com/ligand-discovery/fragment-predictor)|[DOI](https://zenodo.org/records/10838071)
   |---|---|---|

Predict whether your fully-functionalized fragment of interest is likely to be promiscuous or associated with a specific interactome signature. We have predefined 10 interactome signatures capturing high-level biological processes that emerged from our chemoproteomics data
   
### 5. :rocket: **On-the-fly modeling**

   |[Web App](https://5.ligand-discovery.ai) :arrow_upper_right:|[Code Repo](https://github.com/ligand-discovery/on-the-fly-modeling)|[DOI](https://zenodo.org/records/10838098)
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

---

#### FAQ for web apps

1. Interactions web app
   
`Do i have to clear existing text to search for a new Protein?`

**No**. To change selected protein, there is **no** need to select whole existing term or delete or type new. Just place the mouse cursor in the search box and **just start to type new protein!**; old text is automatically cleared

`I search for a gene (example, DDB1) but did not find it in Protein search box`

Names like **caspase** or **ddb1** appear many times in description of proteins, therefore search engine is not able to pick the correct one. Type specific input such as **DNA damage-binding protein 1** or **DDB1 DNA dama..** to find **DDB1**. Search with **UniProt Accession** (Q16531 for DDB1) **is better!**

`I am interested in a specific Fragment (C008) but it is not displayed in the Gen1 search box`

Gen1 Fragment selection menu is dynamically updated based on the selected Protein **and** threshold filters applied. If you are interested in a specific Gen1 Fragment, then clear all filters, i.e., select **'no filter'** option for _P_ values, adjusted _P_ alues and filterSet  (fS) **and/or** select a promiscuous Protein such as **TOMM22**

`Changing the threhold for _P_ values, adjusted _P_ values and filterSet (fS) does not change the plot`

That is correct. **Plots are static**. They are not dynamically updated based on threshold values. Changing the threhold for _P_ values, adjusted _P_ values and filterSet (fS) **only updates the Table**. Pre- set (i.e. default) filterSet (**fS** or **fS2**) were used to create plots

`What was the criteria to label a Protien or Fragment as Promiscuous ?`

**10%** hit/regulated ratio for Proteins and **5%** for Fragments")

`Can i change the order of Gen1 Fragments displayed in the search box menu?`

Order of Fragments displayed in search menu matches the **original** order in the Table. Re-adjusting the table, for example: sort the table based on Foldchange (Fc) values or number of Protein/Fragment hits **will not change the order** of the Fragments in the search menu

Changing the threhold for _P_ values, adjusted _P_ values and filterSet (fS) updates the **original** Table, consequently results in a change in the order of Gen1 Fragment displayed in search menu

`How can i explore second generation (Gen2) Fragment data?`

Gen2 Fragment data is available for only a small subset of Gen1 Fragments. **Gen2 data is automatically displayed** if the selected Gen1 Fragment has elaborates. For example, select **C027** in Gen1 search box

2. Explore Protein-sets app

`How to resolve error message 'More than one input type has been provided!'?`

Please only choose one of the options, i.e. input proteins manually, or select a pre-screened Ligand, or upload a file

4. Fragment Predictor web app

`Explain Promiscuity and Ontology Prediction models`

1. We built two types of Promiscuity models. Three Type 1 (Global) and nine Type 2 (Specific) models 
2. We built 10 Ontology models. 
3. Area Under Receiver Operating Characteristic (AUROC) of > 0.75 is considered a :blue[good model]

|Global | num. Proteins | AUROC
|---|---|---|
Prom-0 | 100+ | :blue[0.837]
Prom-1 | 200+ | :blue[0.800]
Prom-2 | 300+ | :orange[0.713]

|Specific | num. Proteins | num. Fragments | AUROC
|---|---|---|---|
Prom-0-0|5+| < 4 | :blue[0.818]
Prom-0-1|10+| 4 -> 40 | :blue[0.809]
Prom-0-2|50+| > 40 | :blue[0.857]
Prom-1-0|10+| < 4 | :blue[0.771]
Prom-1-1|15+| 4 -> 40 | :blue[0.855]
Prom-1-2|100+| > 40 | :blue[0.858]
Prom-2-0|50+| < 4 | :orange[0.771]
Prom-2-1|100+| 4 -> 40  | :orange[0.743]
Prom-2-2|200+| > 40 | :blue[0.814]

Model name | Ontology | AUROC
|---|---|---|
Sign-0 | Endoplasmic reticulum | :blue[0.872]
Sign-1 | RNA binding | :orange[0.727]
Sign-2 | Lysosome | :blue[0.938]
Sign-3 | Proteasome complex | :orange[0.616]
Sign-4 | Mitochondria | :orange[0.519]
Sign-5 | Nucleous | :orange[0.702]
Sign-6 | Transmembrane transporter | :blue[0.756]
Sign-7 | Microtubule | :orange[0.557]
Sign-8 | Organic acid binding | :orange[0.706]
Sign-9 | Envelope | :blue[0.806]
