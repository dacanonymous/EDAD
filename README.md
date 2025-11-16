# EDAD
## Streaming Anomaly Detection using EDAD

### Dataset Download Instructions

Please download the following datasets manually and place them in the data/ directory.

These datasets come from:
Govorkova, E., Puljak, E., Aarrestad, T., Pierini, M., Woźniak, K. A., & Ngadiuba, J. (2022).
LHC physics dataset for unsupervised New Physics detection at 40 MHz. Scientific Data, 9(1), 118.

##### Dataset Links

###### Training dataset (background):
  https://zenodo.org/records/5046389
###### LQ → bτ signal benchmark dataset:
  https://zenodo.org/records/5055454
###### A → 4 leptons benchmark dataset:
  https://zenodo.org/records/5046446
###### h0→ττ signal benchmark dataset:
  https://zenodo.org/records/5061633
###### h+→τv signal benchmark dataset:
  https://zenodo.org/records/5061688


### Reproducing the Experiments

The results/ and figures/ directories already contain sample outputs.
To fully reproduce the experiments, follow the workflow below:

#### Download datasets
Place all downloaded files under the data/ directory.

#### Run the grid search to obtain the optimal EDAD hyperparameter
Use the notebook:
EDAD_grid_search_LHC_L1T.ipynb

#### Run the experiments
After selecting parameters from grid search, run:
EDAD_Experiment_LHC_L1T.ipynb

#### Generate figures
Once the results are computed, use:
produce_figures.ipynb
to generate ROC curves and TPR/FPR plots.
