## 什么是 dropout

dropout 是指在深度学习网络的训练过程中，对于神经网络单元，按照一定的概率将其暂时从网络中丢弃。dropout 不在推理中使用。

![](https://github.com/steveLauwh/DeepLearning-notebook/raw/master/Basic%20concepts/image/dropout.png)

dropout 有一个重要特性是防止过拟合。

## dropout 率的选择

* 经过交叉验证，隐含节点 dropout 率等于 0.5 的时候效果最好，原因是 0.5 的时候 dropout 随机生成的网络结构最多。
* dropout 也可以被用作一种添加噪声的方法，直接对 input 进行操作。输入层设为更接近 1 的数，使得输入变化不会太大（0.8）。
