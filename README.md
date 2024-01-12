## building-makemore to 'learnmore'
*"makemore takes one text file as input, where each line is assumed to be one training thing, and generates more things like it. Under the hood, it is an autoregressive character-level language model, with a wide choice of models from bigrams all the way to a Transformer (exactly as seen in GPT)."* https://github.com/karpathy/makemore

### What I've learned:

**Lecture 1:** Created a bigram character level language model- learning how to train the model, sample from the model, and evaluate the quality of the model using the negative log likelihood loss. Trained the model in two completely different ways that actually give the same result. The first way just involved counting up the frequency of all the bigrams and normalizing it. The second way involved using the negative log likelihood loss as a guide to optimize the counts matrix/array so that the loss is minimized in a gradient based framework.

**Lecture 2:** Created a Multi-Layer Perceptron (MLP) character level language model following the research paper [Bengio et al. 2003](https://www.jmlr.org/papers/volume3/bengio03a/bengio03a.pdf). Learned about splitting dataset into Train, Validation, and Test splits, finding the ideal learning rate through graphing the loss, constructing minibatches to help converge faster, and overall model hyperparameter tuning and optimization to minimize loss. Otherwise, very straightforward- followed the diagram on Page 6 of the paper.  
