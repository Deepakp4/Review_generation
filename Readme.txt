Optimizing Peer Review Automation: A Section-Specific Evaluation of T5 and PEFT Fine-Tuning


Project Overview
This project focuses on developing an automated system to generate peer reviews for scientific papers using T5-based language models. We leverage the ASAP-Review dataset for training, fine-tuning, and evaluating models to enhance the peer review process. The models compared include a baseline TF-IDF model, Standard T5, and PEFT T5, each evaluated on performance metrics like ROUGE, METEOR, Precision, Recall, and F1 Score.

Project Objectives
Baseline Review Generation: Use TF-IDF extraction for generating initial reviews from scientific papers.
Model Fine-tuning: Fine-tune Standard T5 and PEFT T5 for better review quality, leveraging summaries from multiple sections of the paper.
Evaluation: Use evaluation metrics like ROUGE, METEOR, Precision, Recall, and F1 Score to assess model performance.
Comparison: Compare Standard T5 with PEFT T5 in terms of computational efficiency and performance.
Dataset
Dataset: ASAP-Review dataset, consisting of 8,742 scientific papers and 25,986 associated reviews across various domains.
Data Splits:
Training: 20,757 pairs
Validation: 2,571 pairs
Testing: 2,658 pairs
Sections Extracted: Abstract, Introduction, Methods, Results, Conclusion.
Models
Baseline Model (TF-IDF):

Extracts key sentences from the Introduction section using TF-IDF vectorization.
Standard T5:

Fully fine-tuned model using multiple sections of scientific papers (Abstract, Introduction, etc.) for generating reviews.
PEFT T5:

Uses Parameter-Efficient Fine-Tuning (PEFT) techniques to improve computational efficiency by fine-tuning specific parameters rather than the entire model.
Installation
Requirements
Python 3.8+
PyTorch
Hugging Face Transformers
Scikit-learn