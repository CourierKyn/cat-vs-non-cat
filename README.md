# cat-vs-non-cat

同样是利用 cat-vs-non-cat 数据集，在第一次作业中，只使用一个 Logistic 层实现了 70% 的测试准确率。在这个作业项目中将构造深度神经网络模型，来增加模型的复杂度，提高预测准确率。在 `Deep_Neural_Network_Model.ipynb` 中实现了 DNN 的各个函数模块，在 `Model_Application.ipynb` 中调用 `Deep_Neural_Network_Model.ipynb` 的各个函数模块构造 DNN，对 cat-vs-non-cat 数据集进行训练预测。

**`Deep_Neural_Network_Model.ipynb` 结构如下：**

* 初始化 Weight, bias
* Forward propagation
  * 构造 `[linear -> relu] × (L-1) -> linear -> sigmoid` 的前向传播模型
* Cost function
* Backward propagation
  * 构造 `[linear -> relu] × (L-1) -> linear -> sigmoid` 的前向传播模型
  * 更新权重，偏差

**`Model_Application.ipynb` 结构如下：**

* 构造两层神经网络模型，隐藏层 7 个神经网络单元，2500 次迭代后，Test Accuracy = 0.72
* 构造五层神经网络模型，各层神经网络单元为 `[12288, 20, 7, 5, 1]`， 2500 次迭代后，Test Accuracy = 0.80

## 使用自己的训练集

![](IMG_0760.JPG)
