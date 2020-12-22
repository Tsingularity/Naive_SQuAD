# Naive_SQuAD
This repo contains the data pre-processing and model training code for the following two methods:

### Naive DrQA
We utilize the Document Reader architecture in [DrQA](https://arxiv.org/abs/1704.00051) to predict answer text span in the context for the given questions. But for the context encoding, we only use fixed word embedding and aligned question embedding as inputs.

### Finetune BERT-base
We add a linear classifer on top of BERT output and finetune them together on the given question answering task. The BERT model is Huggingface Transformer's [BERT-base-uncased](https://huggingface.co/bert-base-uncased).
