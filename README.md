# NLP Disaster Tweets Classifier 

This repository contains an end-to-end Natural Language Processing (NLP) pipeline to classify disaster-related tweets using the pre-trained DistilBERT model. The pipeline includes data preprocessing, model fine-tuning with Hugging Face's Trainer, and final predictions. The fine-tuned model achieved an 83% F1-score accuracy on the Kaggle test dataset, demonstrating its effectiveness in classifying tweets as related or unrelated to real disasters.

## Features 
- **Data Preprocessing:** Tokenization, splitting into training and development sets, and padding/truncation for model compatibility.
- **Model Fine-Tuning:** Utilizes DistilBERT (distilbert-base-uncased-finetuned-sst-2-english) for binary classification with custom training configurations.
- **Evaluation Metrics:** Reports accuracy, precision, recall, and F1-score on training and development sets.
- **Custom Callbacks:** Includes a debugging callback to log training progress and early stopping for optimal performance.
- **Final Predictions:** Outputs predictions on test data in a structured CSV format.
- 
## Instructions 
1. Ensure you have the required libraries installed (transformers, datasets, pandas, numpy, scikit-learn)
2. Place the training and test datasets (`train.csv` and `test.csv`) in an appropriate directory
3. Run all code cells sequentially in the script.
4. The final predictions will be saved in a CSV file named `predictions.csv` in the same directory.

## Dependencies 
- **transformers:** For tokenization and fine-tuning the `DistilBERT model`.
- **datasets:** For handling datasets compatible with Hugging Face's Trainer.
- **pandas:** For data manipulation and processing.
- **numpy:** For numerical computations.
- **scikit-learn:** For evaluation metrics such as accuracy, precision, recall, and F1-score.

## Notes 
- Ensure the file paths in the script match the locations of your datasets.
- The training arguments can be adjusted to explore different configurations (e.g., learning rate, batch size, epochs).
- The `random_state = 42` is used throughout to ensure reproducibility.

## Author 
Christina Joslin 

## Acknowledgements 
- Data provided by the [Kaggle Disaster Tweets competition](https://www.kaggle.com/competitions/nlp-getting-started).
- Special thanks to the open-source community for contributing the libraries and tools used in this project.
