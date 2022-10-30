#### 1.《Distributed Reinforcement Learning for Coordinate Multi-Robot Foraging》(2010)

内容：介绍了一种改进智能体更新自己Q函数的方法(D-DCM-Multi-Q)，每个智能体考虑周边其他智能体的Q值对自己进行更新
$$
Q_{k+1, i}\left(s_i, a_i\right)=(1-\alpha) Q_{k, i}\left(s_i, a_i\right)+\alpha\left(R_{k, i}\left(s_i, a_i\right)+\gamma \sum_{j=1}^N f(i, j) V_{k, j}\left(s_i^{\prime}\right)\right)
$$
评价：对自己方法的解释和对应的公式之间存在矛盾，用的话可能要改一改？

