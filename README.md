# Spurious Correlations in Deep Learning

In this project my goal is to create simple settings in which I can 
test the effects of spurious correlations on deep learning models. Briefly, this effect occurs 
when models learn to rely on features of the training data which are correlated with the target, 
but which aren't generalizable in testing or real world datasets. Work from [1] and [2] studies this effect and proposes 
simple last last layer re-training and re-weighting strategies step in order to fix the problem and generalize to new data. 

In this project I focus on creating simple testing grounds to test these strategies upon. Whereas [1] and [2]
relies on image data having spurious features, I adapt the mnist1d data set [2] by generating 
controlled, spurious features. With this I perform tests that 1) illustrate the effects
of spurious correlations and 2) experiment with the strategies from [1] and [2].

All code is documented and done within ```spurious_mnist.ipynb```
And more details about my experiments and results are documented in ```writeup.pdf```

## References
<a href="https://arxiv.org/abs/2204.02937">[1]</a> 
Kirichenko, Ismailov, and Wilson. 
On feature learning in the
presence of spurious correlations. Advances in Neural Information Processing Systems, 35:38516–38532,
2022. 

<a href="https://arxiv.org/abs/2306.11074">[2]</a> 
Qiu, Potapczynski, Izmailov, and Wilson. Simple and fast group
robustness by automatic feature reweighting. In International Conference on Machine Learning,
pages 28448–28467. PMLR, 2023

<a href="https://github.com/greydanus/mnist1d">[3]</a>  Sam Greydanus. Scaling down deep learning, 2020
