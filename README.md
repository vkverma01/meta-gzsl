# Meta-Learning for Generalized Zero-Shot Learning

Learning to classify unseen class samples at test time is popularly referred to as zero-shot learning (ZSL). If test samples can be from training (seen) as well as unseen classes, it is a more challenging problem due to the existence of strong bias towards seen classes. This problem is generally known as \emph{generalized} zero-shot learning (GZSL). Thanks to the recent advances in generative models such as VAEs and GANs, sample synthesis based approaches have gained considerable attention for solving this problem. These approaches are able to handle the problem of class bias by synthesizing unseen class samples. However, these ZSL/GZSL models suffer due to the following key limitations: (i) Their training stage learns a class-conditioned generator using only \emph{seen} class data and the training stage does not \emph{explicitly} learn to generate the unseen class samples; (ii) They do not learn a generic optimal parameter which can easily generalize for both seen and unseen class generation; and (iii) If we only have access to a very few samples per seen class, these models tend to perform poorly. In this paper, we propose a meta-learning based generative model that naturally handles these limitations. The proposed model is based on integrating model-agnostic meta learning with a Wasserstein GAN (WGAN) to handle (i) and (iii), and uses a novel task distribution to handle (ii). Our proposed model yields significant improvements on standard ZSL as well as more challenging GZSL setting. In ZSL setting, our model yields 4.5\%, 6.0\%, 9.8\%, and 27.9\% relative improvements over the current state-of-the-art on CUB, AWA1, AWA2, and aPY datasets, respectively.

## Data Download
Download the data from the address: http://www.robots.ox.ac.uk/~lz/DEM_cvpr2017/data.zip.

Use the CUB attribute provided by this repository; it is CNN-RNN 1024 dimensional learned attribute.

## Reference
```@article{verma2019meta,
  title={A meta-learning framework for generalized zero-shot learning},
  author={Verma, Vinay Kumar and Brahma, Dhanajit and Rai, Piyush},
  journal={Thirty-Fourth AAAI Conference on Artificial Intelligence (AAAI-20)},
  year={2020}
}
```
### Note:
1- Please note that this is not final implementation, this code is mostly the analysis of the result and network, but it help to get the idea and reproduce the result.

2-Code is not clean many line may me redundant, Also comments are not proper. 
