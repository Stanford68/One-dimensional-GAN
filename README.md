# One-dimensional-GAN

GAN生成一维数据
使用需要加载数据，数据形状为[Batch,InputLength,1], 数据长度注意修改inputLength保持一致。
基于tensorflow2.0


新增WAGN-GP版本。


2020.02.23
新增脚本regress.py, 给出了一种处理回归问题的思路：

假设问题为4个已知数据,估计另一个值，则可表述为，

4个已知数据 ---> 生成器 ---> 1个所求数据

[4个已知数据，1个所求数据(真实) ]---> 判别器 

[4个已知数据，1个所求数据(生成) ]---> 判别器
