
BERT Integration for Question Pair Classification

This repository contains a Python implementation for fine-tuning a BERT model to classify question pairs as duplicates or not, using the Quora Question Pairs dataset.

 Features
- Preprocessing 
- Feature Extraction
- Fine-tuning the BERT model for binary classification.
- Training and evaluation loops.
- Saving and loading the fine-tuned model.

 Requirements
- Python 3.8+
- PyTorch
- Transformers (Hugging Face)
- pandas
- scikit-learn

Files
- bert.py: Main script for training and evaluation.
- quora_question_pairs.csv: Dataset file containing question pairs and labels.

 Setup
1. Clone this repository:
bash
   git clone https://github.com/HarshithaTentu/bertintegration.git
   cd bertintegration
 

2. Install dependencies:
 bash
   pip install -r requirements.txt
 

3. Place the `quora_question_pairs.csv` file in the same directory as `bert.py`.

 Usage
Run the training script:
bash
python bert.py


The script will:
1. Load and preprocess the dataset.
2. Fine-tune the BERT model on the question pairs.
3. Save the trained model to `quora_bert_model`.

 Outputs
- Training logs with loss values.
- Validation accuracy after training.
- A fine-tuned BERT model saved in `quora_bert_model`.

 Notes
- Ensure the dataset file is formatted with columns: `question1`, `question2`, `is_duplicate`.
- Modify paths in the code if necessary to point to your dataset file.

 Contributing
Feel free to fork and submit pull requests to improve the project.

