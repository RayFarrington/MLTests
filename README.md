# MLTests

Collection of machine learning projects and Jupyter notebooks created for coursework and experiments. The projects focus on DDoS detection using tabular network flow features and compare different model architectures (MLP, CNN). These notebooks are intended as reproducible analyses and teaching artifacts.

## Notebooks (high-level)
- Notebooks/DDosModel.ipynb : Exploratory Data Analysis (EDA), missing-value investigation, initial preprocessing and baseline model experiments.
- Notebooks/MLPDDosModel.ipynb : Data cleaning, feature engineering, and an MLP (multi-layer perceptron) classification model trained and evaluated on the DDoS dataset.
- Notebooks/MLPvsCNN.ipynb : Direct comparison of MLP and CNN model architectures on the same preprocessed dataset to study whether convolutional layers improve performance.

## Data
- data is from this data set: https://www.kaggle.com/code/atulkumar011/ddos-attack-detection-classification-a03d6b/input

## Reproducing results & notes
- The notebooks read the CSV directly from the repo's data/ directory (raw GitHub link). If you want to work offline, download data/DDOS_Data.csv and update the notebook path.
- Notebooks perform preprocessing steps (median fill for some missing values, log transforms, scaling, feature engineering like bytes_per_packet and tx_rx_ratio_bytes). See each notebook’s EDA and preprocessing sections for exact steps and reasoning.
- For deterministic results, set random seeds in numpy, TensorFlow, and sklearn inside the notebooks prior to model training.
- GPU can speed up training for deep models — Colab/GPU or local CUDA setup recommended if experimenting with larger networks.

## Usage
- These notebooks were created for classes and experiments; feel free to reuse code snippets and adapt preprocessing/model pipelines.

## Contact
Questions or suggestions: raise an issue on the repository or contact the author (Ray Farrington).
