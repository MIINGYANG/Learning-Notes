#### 1.《Distributed Reinforcement Learning for Coordinate Multi-Robot Foraging》(2010)

内容：介绍了一种改进智能体更新自己Q函数的方法(D-DCM-Multi-Q)，每个智能体考虑周边其他智能体的Q值对自己进行更新
$$
Q_{k+1, i}\left(s_i, a_i\right)=(1-\alpha) Q_{k, i}\left(s_i, a_i\right)+\alpha\left(R_{k, i}\left(s_i, a_i\right)+\gamma \sum_{j=1}^N f(i, j) V_{k, j}\left(s_i^{\prime}\right)\right)
$$
评价：对自己方法的解释和对应的公式之间存在矛盾，用的话可能要改一改？

#### 2. 《PD-FAC: Probability Density Factorized Multi-Agent Distributional Reinforcement Learning for Multi-Robot Reliable Search》

内容：解决多机可靠搜索问题，采用无向图的形式，将多机可靠搜索问题定义为了三个子问题

解决了两个网络训练的问题：

1. 联合观测与联合动作随着机器人数量的增加指数增加

   解决方法：引入概率密度因数分解

2. 观测不定长

   解决方法：引入GRU(gated recurrent unit)对状态进行编码，输出定长特征(状态为定长)

网络结构：

![1](images/1.png)







































