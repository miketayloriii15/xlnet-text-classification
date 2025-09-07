# XLNet Text Classification

This repository contains a Jupyter notebook demonstrating how to fine-tune **XLNet** for text classification using the [Hugging Face Transformers](https://huggingface.co/transformers/) library.  
The project trains and evaluates a model on an emotion classification dataset.

---

## Dataset Setup

Place your dataset CSV files in a folder named **`emotions_data`** located in the **same directory** as the Jupyter notebook:

emotions_data/
├── emotion_labels_train.csv
├── emotion_labels_val.csv
├── emotion_labels_test.csv

yaml
Copy code

Each file should contain the text samples and their corresponding labels.

---

## Features

- Uses **XLNet** pretrained model from Hugging Face  
- Tokenization and preprocessing with `transformers`  
- Training with Hugging Face **Trainer API**  
- Evaluation on validation and test sets  
- Computes accuracy and other metrics  
- Runs end-to-end in a single notebook

---

## Installation

It is recommended to use Python 3.9+.

1. Clone this repository:
```bash
git clone https://github.com/your-username/xlnet-text-classification.git
cd xlnet-text-classification
Install the required libraries:

bash
Copy code
pip install torch transformers datasets scikit-learn
(Optional) If running in Jupyter:

bash
Copy code
pip install notebook
Usage
Ensure the dataset is in the emotions_data/ folder.

Open the notebook:

bash
Copy code
jupyter notebook xlnet_text_classification.ipynb
Run the cells to:

Load and preprocess the dataset

Fine-tune XLNet on training data

Evaluate on validation and test sets

Inspect sample predictions

Example Output
During training, you will see logs with loss, accuracy, and evaluation metrics. After completion, the notebook will display model performance on the validation and test sets along with sample predictions.

Notes
XLNet is powerful but resource-intensive. Training is faster with GPU acceleration (CUDA).

The provided dataset paths assume CSV format with text and label columns. Adjust preprocessing if your data differs.

License
This project is open source under the MIT License.
