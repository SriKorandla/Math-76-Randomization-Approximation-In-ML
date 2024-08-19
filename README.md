# Randomization and Approximation in Machine Learning
## Math 76.01, Mathematics in AI Final Project (Warren Shepard, Sri Korandla, Tushar Aggarwal)

### Project Summary:
We were interested by the obsession with perfect prediction algorithms which never make computational errors, and an interest in allowing for room for error. We believed that this would lead to better (and more realistic) predictions and less over-fitting
of models. We tested kNN (sci-kit-learn) against our own approximate kNN (pynndescent package) against each other, and noted a drastic speed increase with very little to no accuracy tradeoff. We next used these as a subroutine for Graph based semi-supervised learning, with models trained on labeled and unlabeled data with a label propogation algorithm implemented from scratch. We tested this on both a small toy synthetic dataset, and MNIST's handwritten digit dataset. k Approximate was actually slightly more accurate, and nearly twice as fast. We then did pruning and randomized pruning masks, which we did through training small neural networks on the MNIST Fashion dataset, and used 5 different pruning approaches. Ultimately, we found that our approach of Fractional Random Threshold Pruning (Selecting a fraction of connections with the smallest weights and pruning a smaller fraction of these) outperformed Threshold Fraction pruning, and all other methods other than no pruning.

### Links to Data Sets:
MNIST data set used for Neural nets notebook, and the graph based supervised learning. We used the handwritten digits, and the fashion data set.
Other data sets used were synthetically created by us for the approximate knn and graph based learning sections as well. 
Links Below: 
https://yann.lecun.com/exdb/mnist/
https://github.com/zalandoresearch/fashion-mnist




### Links to Relevant Research Paper(s) used for Inspiration:

Paper by Li et al on randomized pruning for masking: https://arxiv.org/abs/2310.13183
Paper by Li et al on Pruning on language models: https://arxiv.org/abs/2310.13191
(Inspired by the Randomized Pruning, which we showed could be useful in small models)

Paper by https://www.theoryofcomputing.org/articles/v008a014 inspired us to use pynndescent for our implementation of Approximate nearest neighbors



