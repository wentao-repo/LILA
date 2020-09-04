# LILA
A Pytorch implementation of the LILA framework proposed in our paper "Learning from Incomplete Labeled Datavia Adversarial Data Generation".


Brief Introduction

Positive and unlabeled (PU) learning aims to obtain a well-performed classifier via an incomplete binary training set, in which only a part of labels of one category is known while the rest are unknown. 
However, in many real-world applications such as image recognition, the collected data samples often involve more than two categories.
Moreover, due to some practical reasons, only a small portion of the collected samples might have associated labels, and these labeled samples cannot always cover all the possible categories. 
We refer to this type of data as \emph{incomplete labeled data} and, in this paper, we first formally define the incomplete labeled data learning problem and then aim to tackle it via adversarial data generation. Specifically, we propose a novel generative framework LILA, which is able to produce synthetic labeled samples for both partially labeled categories and unlabeled categories.
To enforce that the generated samples for unlabeled categories can associate with correct labels, we integrate two active learning processes into the LILA framework for selecting unlabeled samples in the collected sample set to query their labels effectively.
After LILA has been well trained, a classifier can be trained on the balanced augmented data set consisting of both generated synthetic labeled samples and original labeled samples. 
Extensive experiments on real image data demonstrate the effectiveness of our proposed framework. 
