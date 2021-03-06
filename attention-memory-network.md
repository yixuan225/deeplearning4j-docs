---
title: A Beginner's Guide to Attention and Memory Networks
layout: default
---

# A Beginner's Guide to Attention and Memory Networks

At any given moment, our minds concentrate on a subset of the total information available to them. (Fwiw, this is also true for artificial neural networks using an attention mechanism.) For example, you are reading these words as a larger world flows around you: maybe you're in a room with traffic coursing outside, maybe you're in a plane and the pilot is making another annoying announcement about turbulent, but your focus is **here**. 

Attention is, in a sense, the mind's capital, the chief resource it can allocate and spend. Algorithms can also allocate attention, and learn how to do it better, by adjusting the weights they assign to various inputs. It is used for speech recognition, machine translation, reasoning, image captioning, summarization, and visual identification of objects.

"Attention" is defined as the "active direction of the mind to an object", or more literarily as "giving heed".<sup>[1](#one)</sup> The word describes the mind's ability to allocate consideration unevenly across a field of sensation, thought and proprioception, to focus and bring certain inputs to the fore, while ignoring or diminishing the importance of others.  This is important, because the field of sensation is wide, and the mind's bandwidth to process information is narrow, and some inputs are indeed more important that others, with regard to any given goal. 

## Credit Assignment Among Available Features

The fundamental task of all neural networks is *credit assignment*. Credit assignment is allocating importance to input features through the weights of the neural network's model. Learning is the process by which neural networks figure out which input features correlate highly with the outcomes the net tries to predict, and their learnings are embodied in the adjusted quantities of the weights that result in accurate decisions about the data they're exposed to. 

But there are different ways to structure and channel the relationship of input features to outcomes. [Feed-forward networks](./neuralnet-overview.html) are a way of establishing a relationship between all input features (e.g. the pixels in a picture) and the predictions you want to make about the input (e.g. this photo represents a dog or a cat), and doing so all at the same time. 

When we try to predict temporal sequences of things, like words in a sentence or measurements in a time series (e.g. temperatures or stock prices), we channel inputs in other ways. For example, a [recurrent neural network like an LSTM](./lstm.html) is often used, since it takes account of information in the present time step as well as the context of past time steps. Below is one way to think about how a recurrent network operates: at each time step, it combines input from the present moment, as well as input from the memory layer, to make a decision about the data. 

![Alt text](./img/recurrent_network.png)

An attention mechanism takes into account the input from several time steps, say, to make one prediction. And just as importantly, it accords different weights, or degrees of importance, to those inputs, reflected below in the lines of different thicknesses and color. 

![Alt text](./img/attention_mechanism.png)

## Navigating Complex Spaces

If you tell your self-driving car to park itself "under the elm tree near the yellow house two blocks away where the curb is unmetered", how can the machine understanding the important parts of that complex and ambiguous instruction and map them to the physical world, which is submerged in noise? 

WIP

### <a name="beginner">Further Reading on Attention Networks</a>

* [Attention and Memory in Deep Learning and NLP](http://www.wildml.com/2016/01/attention-and-memory-in-deep-learning-and-nlp/)
* [Memory, attention, sequences](https://towardsdatascience.com/memory-attention-sequences-37456d271992)
* [Attention Mechanism](https://blog.heuritech.com/2016/01/20/attention-mechanism/)
* [Attention and Augmented Recurrent Neural Networks](https://distill.pub/2016/augmented-rnns/)
* [Attention in Neural Networks and How to Use It](http://akosiorek.github.io/ml/2017/10/14/visual-attention.html)
* [How Does Attention Work in Encoder-Decoder Recurrent Neural Networks](https://machinelearningmastery.com/how-does-attention-work-in-encoder-decoder-recurrent-neural-networks/)
* [Show, Attend and Tell: Neural Image Caption Generation with Visual Attention](https://arxiv.org/abs/1502.03044)
* [Recurrent Models of Visual Attention](https://arxiv.org/abs/1406.6247)
* [End-To-End Memory Networks](https://arxiv.org/abs/1503.08895)
* [Sequence to Sequence Learning with Neural Networks](https://arxiv.org/abs/1409.3215)
* [Learning Phrase Representations using RNN Encoder-Decoder for Statistical Machine Translation](https://arxiv.org/abs/1406.1078)
* [Neural Machine Translation by Jointly Learning to Align and Translate](https://arxiv.org/abs/1409.0473)
* [Effective Approaches to Attention-based Neural Machine Translation](https://arxiv.org/abs/1508.04025)
* [Attention Is All You Need](https://arxiv.org/abs/1706.03762)
* [Video Lecture 10: Neural Machine Translation and Models with Attention (Stanford)](https://www.youtube.com/watch?v=IxQtK2SjWWM)
* [Video Lecture 8 - Generating Language with Attention](https://www.youtube.com/watch?v=ah7_mfl7LD0)


### <a name="beginner">Other Machine Learning Tutorials</a>

* [Multilayer Perceptron (MLPs) for Classification](./multilayerperceptron.html)
* [Eigenvectors, Eigenvalues, Covariance, PCA and Entropy](./eigenvector.html)
* [LSTMs and Recurrent Networks](./lstm.html)
* [Word2vec, Doc2vec & GloVe: Neural Embeddings and NLP](./word2vec.html)
* [Introduction to Deep Neural Networks](./neuralnet-overview.html)
* [Deep Convolutional Networks](./convolutionalnetwork.html)
* [Generative Adversarial Networks (GANs)](./generative-adversarial-network.html)
* [Deep Reinforcement Learning](./deepreinforcementlearning.html)
* [Quickstart Examples for Deeplearning4j](./quickstart.html)
* [ND4J: A Tensor Library for the JVM](http://nd4j.org)
* [MNIST for Beginners](./mnist-for-beginners.html)
* [Glossary of Deep-Learning and Neural-Net Terms](./glossary.html)
* [Restricted Boltzmann Machines](./restrictedboltzmannmachine.html)
* [Inference: Machine Learning Model Server](./machine-learning-server.html)
* [AI vs. Machine Learning vs. Deep Learning](./ai-machinelearning-deeplearning.html)
* [Convolutional Networks (CNNs)](./convolutionalnetwork.html)
* [Multilayer Perceptron (MLPs) for Classification](./multilayerperceptron)
* [Graph Data and Deep Learning](./graphanalytics.html)
* [Symbolic Reasoning (Symbolic AI) & Deep Learning](./symbolicreasoning.html)
* [Markov Chain Monte Carlo & Machine Learning](/markovchainmontecarlo.html)
* [Neural Networks & Regression](./logistic-regression.html)
* [Introduction to Decision Trees](./decision-tree.html)
* [Introduction to Random Forests](./random-forest.html)
* [Open Datasets for Machine Learning](./opendata.html)

<a name="one">1)</a> *"Heed", in turn, is related to the German hüten, "to guard or watch carefully".*
