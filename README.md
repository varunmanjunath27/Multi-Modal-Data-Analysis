# Group 21 — Mobile Screen and Text Retrieval
# Varun Manjunath
#Student ID: a1947566

## How to run the program
#Steps

1. Open the project on google colab (.ipynb) notebook.
2. Select Runtime and Change runtime type to T4 GPU.
3. Run the first setup cells to install. The notebook installs its required packages and downloads the dataset directly from link. 
If Colab requests a restart, restart and rerun the setup cells.
4. Continue through the data exploration and cleaning cells. Check the 80-screen manual-review section: inspect the screenshots, 
set `REVIEW_COMPLETED` truthfully 
and update FLAGGED_SCREEN_IDS to match the screens actually flagged. 
Do not assume the IDs prefilled in an executed notebook apply to a new run.
5. Run the remaining cells in order to train and compare the models and view the results.

## What the notebook does

- Checks and cleans screenshot, caption and app metadata.
- Uses pretrained models ResNet-50 and BERT for feature extraction.
- Compares Ridge regression, early fusion, contrastive learning and a hybrid reranker.
- Reports Recall@1/5/10, MRR, training/validation behaviour and retrieval examples.