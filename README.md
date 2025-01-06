# sarcasm-embedding-exp

This repo evaluates the impact of different text embedding methods on classifier performance.  It uses a consistent machine learning model tuning strategy across all experiments. Models are trained on a [dataset](https://www.kaggle.com/code/nilanml/detecting-sarcasm-using-different-embeddings) of 1,000 labeled data points and tested on a separate set of 25,000 labeled data points to determine which embedding strategy best captures the underlying data structure and promotes generalization.

The following embedding methods are evaluated:
* Tokenization
* BERT
* Various [sentence-transformers](https://www.sbert.net/) embeddings
* Mistral 7B as an encoder
* Mistral 7B as a classifier (prompt LLM to determine if headline is parody or news)
* Gemini 1.5 Flash as a classifier
