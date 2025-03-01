# Math-Question-Classification

## Introduction
This project is a part of the course "Natural Language Processing" at IITMZ. The goal of this project is to classify mathematical questions into different categories. The dataset used for this project is in "/data/post-processed/combined.csv" which is a collection of mathematical questions from math textbooks. The dataset contains questions from different mathematical topics like algebra, calculus, geometry, etc. The task is to classify the questions into these categories.

## Dataset
The data is in the "/data" folder. The data contains two folders: "pre-processed" and "post-processed". The "pre-processed" folder contains the original data files and the "post-processed" folder contains the post-processed data files. The data extraction is done in the "extractData.ipynb" notebook. The data files are in CSV format.

The "pre-processed" folder contains the LaTeX and PDF files of 3 math textbooks (Book1, Book2, Book3).

The "post-processed" folder contains the extracted data from the LaTeX and PDF files. There are 3 separate files storing the questions extracted and their classes: "questions_with_chapters.json", "cleaned_math_questions.json", "book3.csv". The combined data is stored in the "combined.csv" file.

The dataset contain the following columns:
- "question": The mathematical question
- "topic": The topic of the question

## Pre-processing
The data is pre-processed to remove any unwanted characters, numbers, and special characters. The pre-processed data is stored in the "post-processed" folder. The pre-processing is done using the "pre.ipynb" notebook.

## Model
The BERT models fine-tuning is done in the "Finetuning.ipynb" notebook. Here, BERT models: BERT, MathBERT, and BERT-Tiny are fine-tuned on our dataset. The attention maps of the models before finetuning are also visualized in this notebook. The models are fine-tuned using the Hugging Face Transformers library. 

---

## For more details, check out this [presentation](https://www.canva.com/design/DAGgQnMn_1M/e_bIbQ1eKcsS5iedKhfmow/view?utm_content=DAGgQnMn_1M&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h7284341ff2).
