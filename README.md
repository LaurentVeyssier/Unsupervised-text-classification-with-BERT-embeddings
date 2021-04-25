# Unsupervised-text-classification-with-BERT-embeddings
Use embeddings to classify text based on multiple categories defined with keywords


This notebook is based on the well-thought project published in towardsdatascience which can be found [here](https://towardsdatascience.com/text-classification-with-no-model-training-935fe0e42180). The detailed original code from the author can be found [here](https://github.com/mdipietro09/DataScience_ArtificialIntelligence_Utils/blob/master/natural_language_processing/example_text_classification.ipynb). It required a bit of adaptation to make it work as per the article. 

# Objective

Use word embeddings and cosine similarity to classify text without model training. The idea is to find similarities between pieces of text and categories (labels) defined using keywords.

# Model

The notebook uses BERT word embeddings (pretrained tensorflow version). BERT is a bidirectional transformers architecture able to associate a different embedding to a same word depending on the sourrounding context (usual example is 'river *bank*' vs 'money *bank*').

# Dataset

The notebook uses news articles (over 50k samples) and we can compare the model performance vs known labels.

# Performance

The performance achieved is not very good (see confusion matrix) however it could be potentially improved as the dictionaries used to define the categories are fine-tuned. This is still an very interesting approach when there is no labeled dataset available to train a multiclass classification model.
