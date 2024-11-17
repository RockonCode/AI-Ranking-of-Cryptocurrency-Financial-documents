
# AI-Ranking-of-Cryptocurrency-Financial-documents

## Overview
The goal of this Project is to check out the efficacy of the Retrieval augmented generation
(RAG) AI technology entailed with ranking financial documents over the cryptocurrency
domain by utilizing Three models within the framework (ColBert, T5, and Crossencoder) to
evaluate each of these model performances relative to the human ranking of cryptocurrency-
based on financial news content.

## Table of Contents
- [Project Description](#project-description)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [implementation](#implementaion)
- [Evaluation Metrics](#evaluation metrics)

## Project Description
This project aims to develop and evaluate a Retrieval-Augmented Generation (RAG) framework for ranking cryptocurrency-related financial news articles. The research involves a comprehensive literature review of RAG frameworks, followed by the manual compilation and preprocessing of a detailed dataset of news articles, including headlines, full text, and mentions of cryptocurrencies like Bitcoin, Ethereum, Binance Coin, Ripple, and Solana. The RAG model will be implemented using ColBERT, T5, and Crossencoder models to identify the top 20 most relevant documents for specific cryptocurrency financial queries. Performance will be assessed using metrics such as NDCG, MAP, Recall@K, MRR, and Precision@K. A comparative analysis will be conducted to evaluate and identify the best model for effectively ranking financial documents within this domain.

## Features
- RAG-based document analysis
- Data Preprocessing: Cleaning and transforming raw data into a suitable format for modeling.
- Feature Engineering: Selecting and creating relevant features for improved model performance.
- Model Training: Implementing and training various machine learning algorithms.
- Model Evaluation: Assessing model performance using appropriate metrics.
- Multi-model evaluation framework:
  - ColBert implementation
  - T5 model integration
  - Crossencoder analysis
- Comparative performance metrics

## Installation
### Prerequisites
- Python
- Jupyter Notebook

### Setup
1. Clone the repository
```bash
https://github.com/RockonCode/AI-Ranking-of-Cryptocurrency-Financial-documents.git
```
2.  Navigate to the project directory:
```bash
cd AI-Ranking-of-Cryptocurrency-Financial-documents
```
3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage
#### Place your dataset in the same directory as your main code file
Here is a simple three-step process to run an `.ipynb` file:

### Step 1: Install Jupyter Notebook
If you haven’t already, install Jupyter Notebook. Open your command prompt (or terminal) and type:
```bash
pip install notebook
```

### Step 2: Launch Jupyter Notebook
Navigate to the directory containing your `.ipynb` file using the command line. Then, launch Jupyter Notebook by typing:
```bash
jupyter notebook
```
This command will open Jupyter in your default web browser.

### Step 3: Open and Run the Notebook
1. In the Jupyter interface, browse to the folder containing your `.ipynb` file and click on the file to open it.
2. To run the code in a cell, click the "Run" button or press `Shift + Enter`. Repeat this for each cell, or go to *Kernel* > *Restart & Run All* to run all cells in sequence.

You can now interact with and run your Jupyter Notebook file!


## Data
#### The Dataset used in this project is created manually. 
The dataset used in this project contains information about Cryptocurrency Financial articles. It includes features such as:

- Link
- Heading
- Full Lenght articles
- Cryptocurrency type
Ensure that the data is in the correct format and located in the data/ directory.

## implementation
To implement the study's objectives, three models—ColBERT, T5, and Crossencoder—are chosen for their effectiveness in information retrieval and document ranking. ColBERT (Contextualized Late Interaction over BERT) is used for its ability to retrieve and rank documents efficiently while preserving contextual information, ensuring an accurate interpretation of cryptocurrency-related financial news. T5 (Text-To-Text Transfer Transformer) is selected for its suitability in text-to-text generation and ranking within the RAG framework. The Crossencoder model is incorporated for its strength in classifying sentence pairs and measuring document-query similarity. Integrating these models into the RAG framework allows for a systematic comparison of their roles and performance, complemented by human evaluation, to address the research question and achieve the study's goals.

## Evaluation Metrics
The below metrics help to assess ranking systems based on the various parameters of
ranking quality, including relevance, position, and overall performance.

#### Normalized Discounted Cumulative Gain (NDCG): 
NDCG is a ranking measure that
compares the actual order of results provided by a search or recommender system with an
ideal order. It takes into account both the importance of an item and its position in the list,
giving more weights to items that are ranked higher. NDCG is a scale from 0 to 1 where 0 is the worst possible ranking and 1 is the best
possible ranking and is useful for comparing different ranking approaches.
#### Mean Average Precision (MAP):
 MAP is one of the ranking statistics that estimate the
average precision for a given set of recall levels. It computes the precision for each of the
retrieved relevant items and then takes the average of all the precision values of the queries
. MAP is especially suitable for assessment of systems where the
amount of pertinent items is limited.
#### Recall@K: 
It is the ratio of the number of retrieved relevant items within the top K results
to the total number of relevant items. It is based on the possible to achieve the high
precision of the system in identifying all the items that are related to the query irrespective
of their rank.
#### Mean Reciprocal Rank (MRR):
MRR estimates the mean of the reciprocal ranks of the
first relevant elements in a list of ranks. It concentrates on the rank
of the first relevant item, the higher the MRR the more relevant items appear at the
beginning of the list.
#### Precision@K: 
The Precision@K defines the ratio of the relevant items to the total number
of retrieved items at the top K. It determines the extent of recovery of the items identified
by the ranking system as relevant.
#### Cosine similarity: 
It is a measure that is used to find the similarity between two vectors
in an inner product space even when the vectors are of different length. It is determined
as the ratio of the dot product of the vectors to the product of their magnitude.
