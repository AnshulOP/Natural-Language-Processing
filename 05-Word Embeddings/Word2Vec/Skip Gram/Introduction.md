                                                              Skip Gram
Skip-gram is a type of Word2vec model that learns word embeddings by predicting the context words given a target word. The model tries to learn the distribution of the context words around a target word by optimizing the probabilities of the context words.

In Skip-gram, given a target word, the model generates training examples containing the target word and a nearby context word. It then uses these examples to learn the probability distribution of the context words given the target word. The model then uses this probability distribution to generate embeddings for the target word.

In contrast to CBOW (Continuous Bag of Words), the Skip-gram model tries to predict context words from the target word. This can be useful in situations where a target word has multiple senses or meanings, as the model can learn to distinguish between them by looking at the different contexts in which the target word appears.

The Skip-gram model has an input layer, a hidden layer, and an output layer. The input layer contains a one-hot encoded vector representing the target word. The hidden layer contains the word embeddings, which are learned during training. The output layer contains a probability distribution over all the words in the vocabulary, with each word represented by a softmax output node.

Skip-gram is generally better suited for larger datasets and less frequent words, as it treats each word occurrence as a new training example. It is also more computationally expensive than CBOW, as it has to train more softmax output nodes.                                                              
