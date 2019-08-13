# Fake-or-Real-News

In this repository, we build models to spot fake and real news based on the news' content.

The first model we build from scratch is a bidirectional LSTM with an attention mechanism followed by a fully connected layers as a decoder. For this model, we tokenize the texts into words and then perform word embeddings using pre-trained word embeddings GloVe. We use torchtext for data preparation for feeding our model. After 20 epochs of training, we obtained a quite decent accuracy score though the model seemed to overfit.

In the second model, instead of word embeddings, we perform sentence embeddings using pre-trained model InferSent. We also add the same attention mechanism as the one in the first model to this model. We observe that after 20 epochs of training, the accuracy does not improve much, but we expect the accuracy will continue to rise if we train the model for more epochs. For more details of InferSent, please refer to https://github.com/facebookresearch/InferSent.
