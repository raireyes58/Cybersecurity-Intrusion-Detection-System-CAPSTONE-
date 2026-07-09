## data/

This folder is intentionally empty in the repository.

The dataset is downloaded automatically when the notebook runs
(Step 2.2), via `kagglehub.dataset_download()`, from:

Source: https://www.kaggle.com/datasets/dnkumars/cybersecurity-intrusion-detection-dataset

This avoids committing a large data file to version control and
ensures the notebook always pulls the current dataset version.

Requirement: a valid Kaggle API key at `~/.kaggle/kaggle.json`
(see https://www.kaggle.com/docs/api for setup instructions).
