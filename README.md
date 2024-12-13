 GPT-2 Theme-Based Lyrics Generation and Sentence-BERT + BiLSTM

Overview
This repository contains two projects for theme-based lyrics generation:
1. GPT-2 Theme-Based Lyrics Generation: Utilizes a fine-tuned GPT-2 model to generate lyrics for specific artists and themes.
2. Sentence-BERT + BiLSTM: Combines Sentence-BERT embeddings with a BiLSTM model to generate coherent lyrics based on artist and theme.

- Prerequisites
-Software and Libraries
Ensure the following are installed:
- Python 3.8 or higher
- Jupyter Notebook
- Required Python libraries (install using `pip`):
  bash
  pip install torch transformers numpy pandas scikit-learn nltk matplotlib tensorflow
  

Hardware
- A GPU is recommended for faster training and inference.

-Running the Projects

1. GPT-2 Theme-Based Lyrics Generation
 Steps to Execute:
1. Open the notebook `GPT2_Theme_Based_Lyrics_Generation.ipynb` in Jupyter Notebook.
2. Ensure the dataset is structured in the following format:
   - Each artist's data should be stored in separate text files.
   - Themes should be categorized within these files.
   - Make sure to add the data according to the specified folder paths in the notebook.
3. Follow the cells step-by-step:
   - Load the data.
   - Fine-tune the GPT-2 model.
   - Generate lyrics using the specified artist, theme, and seed phrase.
4. Evaluate the generated lyrics using BLEU and ROUGE metrics.

Output:
- Generated lyrics will be displayed in the notebook.
- Evaluation scores will be printed for each generation.

---

2. Sentence-BERT + BiLSTM
Steps to Execute:
1. Open the notebook `Sentence_BERT_+_BiLSTM.ipynb` in Jupyter Notebook.
2. Prepare the dataset:
   - Structure similar to GPT-2, with artist and theme categorizations.
   - Make sure to add the data according to the specified folder paths in the notebook.
3. Follow the cells step-by-step:
   - Load the data and generate Sentence-BERT embeddings.
   - Train the BiLSTM model with the embeddings.
   - Use a seed phrase to generate lyrics based on the artist and theme.
4. Evaluate the lyrics using BLEU and ROUGE metrics.

Output:
- Generated lyrics will be displayed in the notebook.
- Evaluation scores will be provided.

 Notes
- Ensure all required datasets are preprocessed and stored in the appropriate directory.
- Modify hyper parameters in the code cells as needed for optimal performance.
- Use GPU for training-intensive steps.

Troubleshooting
- If you encounter memory issues, reduce the batch size or sequence length.
- Ensure the required libraries are installed with compatible versions.