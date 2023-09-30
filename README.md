Data source: https://github.com/sem-tab-challenge/2023/blob/main/datasets/WikidataTables2023R1.tar.gz

Valid/gt: ground truth for CEA, CTA, and CPA, provided by original data source.

Valid/tables: table data

Valid/targets: target CSV files

References:
https://github.com/alan-turing-institute/SemAIDA/tree/master/AAAI19/exp_T2D/
https://github.com/ernestojimenezruiz/tabular-data-semantics-py/blob/master/TabularSemantics/src/kg/

Requirements:
Pre-trained word2vec model by Wikipedia Dump: https://drive.google.com/open?id=1d_xrUPRLQjpcZrlm_cpKJO3jWBFKYhcl

Software & Libraries:
python 3.11.4
pandas 2.1.0
gensim 4.3.1
sparql-client 3.8
tensorflow 2.13

Steps:
1. Get Ground truth and lookup new entities - colnet2.0-gt&lookup.ipynb
2. Training the CNN model - colnet2.0-cnntraining.ipynb
3. Prediction - CNN, Lookup and Ensemble - colnet2.0-prediction.ipynb
4. Evaluate the precision, recall and f1 scores - colnet2.0-evaluation.ipynb
