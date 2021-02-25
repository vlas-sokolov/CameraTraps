This repository contains the code, models, and instructions to run active deep learning animal identification as described in the following paper:

Norouzzadeh, Mohammad Sadegh, Dan Morris, Sara Beery, Neel Joshi, Nebojsa Jojic, and Jeff Clune. "A deep active learning system for species identification and counting in camera trap images." Methods in Ecology and Evolution, 12(1), 150-161 (2021) (https://besjournals.onlinelibrary.wiley.com/doi/abs/10.1111/2041-210X.13504).

# train_embedding.py

This script could be used to learn an embedding model for a given dataset or set of datasets using either triplet, constrastive, or cross entropy loss.
Please refer to the command line arguments and the comments inside the code for further details.
a pretrained embedding model trained on combination of eMammal and CCT datasets is available for download here:
[Base Embedding Model](https://drive.google.com/file/d/1aSprcjmYmZREjQACeCNB-AH9UWfJxEXG/view?usp=sharing)

# run_active_learning.py

This script runs the active learning model on a given dataset. The algorithm starts with 1,000 randomly selected queries and then actively choose the other labels to be labeled by the oracle. This scripts does not consider an oracle in the loop for labeling. Instead, it simulates an oracle by using pre-labeled samples. For further details, please refer to the command line arguments and the comments inside the code.

The snapshots of the model after using 30,000 queries for the Snapshot Serengeti and NACTI datasets are available here:

[Snapshot Serengeti](https://drive.google.com/file/d/1IhD-GY6uEOMROuOkps9UJVBFmGYXiSqB/view?usp=sharing)

[NACTI](https://drive.google.com/file/d/1nhS-83rK4P_ZS07yizZXEFPXL22H7z-Z/view?usp=sharing)
