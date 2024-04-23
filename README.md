# Spurious Correlations in Deep Learning

In this project my goal is to create simple settings in which I can 
test the effects of spurious correlations on deep learning models. Briefly, this effect occurs 
when models learn to rely on features of the training data which are correlated with the target, 
but which aren't generalizable in testing or real world datasets. [1] Studies this effect and proposes 
a simple last last layer re-training step in order to re-weight and generalize to new data. 

In this project I focus on creating simple testing grounds to test this upon. Whereas [1]
relies on image data having spurious features, I adapt the mnist1d data set [2] by generating 
controlled spurious features. With this I will perform tests to describe the effect and validate the work from [1].

## References
<a href="https://arxiv.org/abs/2204.02937">[1]</a> 
Kirichenko, Ismailov, Wilson. 
On feature learning in the
presence of spurious correlations. Advances in Neural Information Processing Systems, 35:38516–38532,
2022. 

<a href="https://github.com/greydanus/mnist1d">[2]</a>  Sam Greydanus. Scaling down deep learning, 2020
