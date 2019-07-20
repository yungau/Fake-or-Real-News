# Fake-or-Real-News

In this repository, we build models to spot fake and real news based on the news' content.

The first model we build from scratch is a bidirectional LSTM with an attention mechanism followed by a fully connected layers as a decoder. For this model, we tokenize the texts into words and then perform word embeddings using pre-trained word embeddings GloVe. We use torchtext for data preparation for feeding our models.

In the second model, instead of word embeddings, we perform sentence embeddings using pre-trained model InferSent. We also add the same attention mechanism as the one in the first model to this model. For more details of InferSent, please refer to https://github.com/facebookresearch/InferSent.
