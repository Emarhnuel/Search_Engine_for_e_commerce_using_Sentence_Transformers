# Search_Engine_for_e_commerce_using_Sentence_Transformers

This project implements a Sentence Transformer-based model for improving search engine performance in an e-commerce setting. It leverages the KDD Cup 22 dataset for training and evaluation.

## Prerequisites
Google Colab Setup:

1. **Create a new Colab notebook**.

2. **Install required libraries**:

```
Bash

!pip install transformers datasets tensorflow tensorflow-probability
```

## Data Acquisition:

1. **Login to aicrowd-cli**:

```
Bash

!aicrowd login

```

2. **Download the KDD Cup 22 dataset**:
```
Bash

!aicrowd dataset download -c esci-challenge-for-improving-product-search
```

3. **Unzip the downloaded files within Colab (refer to notebook cells for specific paths)**.

# Code Structure
1. **data_preparation.py: Loads, cleans KDD Cup data, creates CSV splits with product title retrieval logic.**
2. **model.py: Defines the Transformer model (TFAutoModel), builds the Sentence Transformer with custom loss functions and training loop.**
3. **inference.py: Demonstrates loading embeddings, similarity calculations, and retrieving relevant products based on a query.**


# Usage
1. **Run data preparation**:
```
Bash

!python data_preparation.py
```

2. **Train the model:**
```
Bash

!python model.py
```

3. **Perform product search inference:**
```
Bash

!python inference.py
```
