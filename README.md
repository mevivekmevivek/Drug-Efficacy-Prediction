# Drug-Efficacy-Prediction

The Drug Efficaccy ppt has more details about the datasets, Model architecture(slide 13)

1) The drug features are extracted using SMILES and PaDel Library in python
2) GDSC dataset is the base dataset with Drug, Cell Line and Response(LN IC50)
3) RNA and Copy Number Variations are used as Cell Line features
4) The dimensionality of the RNA and Copy Numbers datasets is reduced using Autoencoders.

Datsets : GDSC drug response datset, CCLE dataset

![Model Arcitecture](https://user-images.githubusercontent.com/10832311/142761702-d244eebd-afba-41ce-a311-bb6914dc08f3.png)

Notebook Descriptions
CCLE Model : The drug efficacy predictions using the CCLE dataset
Drug efficacy Predictions: MOdels build on the single omics and multiomics datasets
Drug_feature_extraction: Using the SMILES of Drugs and Padel library, we extracted the features of the drug
Drug_autoencoded : The extracted features of the drugs are encoded into 50 new features
RNA_autoencoded: The mRNA expressions of each cell line are used as cell line features in the GDSC dataset. The mRNA dataset had over 37K dimensions. The dimensionality is reduced by encoding these fetaures into 100 fetaures.
Response Predictionc : Final models on singe omics and multiomics datasets

