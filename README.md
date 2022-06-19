# Bioinformatics Tool for Drug Discovery 
The bioactivity prediction tool web app was created to quickly verify if a molecule of interest could be a potential candidate in the inhibition of the target protein, hepatocyte growth factor receptor (HGFR). 
---
To make a prediction of the bioactivity of the molecule(s) of interest, a Random Forest model was built. The model was trained and tested using a 80/20 training/testing ratio, with low variance threshold set at 0.1 for the independent features. The model utilized dataset containing compounds with recorded bioactivity values; the dataset was filtered and retrieved from the ChEMBL database. 

The web app takes user input in the form of a .txt file containing the ChEMBLid and SMILES of the molecule(s) of interest. The molecular descriptors and PubChem fingerprints are then calculated for the molecule(s) of interest using the PaDEL-Descriptor software. The webapp was created using Streamlit ([link to code](https://github.com/sara-then/bioactivity_app_streamlit/blob/0156364cbdf17e1f9171ba671fd016d80bc3a664/app.py)).

---
### Credits: 

#### This project was created by Sara Then with inspiration and guidance from Chanin Nantasenamat ([dataprofessor](https://github.com/dataprofessor)) and the Bioinformatics from Scratch series. 
---
### References:

[ChEMBL database](https://www.ebi.ac.uk/chembl/)

[PaDEL-Descriptor software](http://www.yapcwsoft.com/dd/padeldescriptor/)
