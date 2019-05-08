# [cluster](https://github.com/tfzoo/cluster) 
[![sites](tfzoo/tfzoo.png)](http://www.tfzoo.com)
####   qitas@qitas.cn
### [简介](https://github.com/tfzoo/cluster/wiki) 

聚类是一种无监督学习任务，该算法基于数据的内部结构寻找观察样本的自然族群（即集群）。

因为聚类是一种无监督学习（数据无标注），通常使用数据可视化评价结果。

### [参考](tfzoo/) 

#### [K-means](https://github.com/src-d/kmcuda) 

 K-means算法是最为经典的基于划分的聚类方法，是十大经典数据挖掘算法之一。K-means算法的基本思想是：以空间中k个点为中心进行聚类，对最靠近他们的对象归类。通过迭代的方法，逐次更新各聚类中心的值，直至得到最好的聚类结果。

* 优点： 速度快，计算简便 
* 缺点： 我们必须提前知道数据有多少类/组。

K-Medians是与K-Means类似的一种变体，它是通过计算类中所有向量的中值，而不是平均值，来确定簇的中心点。

这种方法的优点是对数据中的异常值不太敏感，但是在较大的数据集时进行聚类时，速度相对于K-Means较慢，造成这种现象的原因是这种方法每次迭代时，都需要对数据进行排序。

#### [DBSCAN](https://github.com/mhahsler/dbscan) 

DBSCAN（Density-Based Spatial Clustering of Applications with Noise,具有噪声的基于密度的聚类方法）是一种基于密度的空间聚类算法。该算法将具有足够密度的区域划分为簇(即要求聚类空间中的一定区域内所包含对象的数目不小于某一给定阈值)，并在具有噪声的空间数据库中发现任意形状的簇，它将簇定义为密度相连的点的最大集合。

在DBSCAN算法中将数据点分为一下三类： 
* 核心点：在半径Eps内含有超过MinPts数目的点 
* 边界点：在半径Eps内点的数量小于MinPts，但是落在核心点的邻域内 
* 噪音点：既不是核心点也不是边界点的点 

####  [Hierarchical](https://github.com/richliao/textClassifier) 

层次聚类算法有两种实现思想，一种是初始时将每个待聚类的数据样本视为一个cluster,采用合并的方式，每次合并两个"距离"最近的cluster，直到合并成一个cluster为止(当然可以在达到自己设定想得到的cluster个数时终止迭代)；另一种刚好与第一种相反，初始时将所有的数据样本视为一个cluster,采用分解的方式。

该算法初始时，将每个点作为一个簇，每一步合并两个最接近的簇。即使到最后，对于噪音点或是离群点也往往还是各占一簇的，除非过度合并。

对于这里的“最接近”，有下面三种定义。我在实现是使用了MIN，该方法在合并时，只要依次取当前最近的点对，如果这个点对当前不在一个簇中，将所在的两个簇合并就行：

* 单链(MIN):定义簇的邻近度为不同两个簇的两个最近的点之间的距离。
* 全链(MAX):定义簇的邻近度为不同两个簇的两个最远的点之间的距离。
* 组平均：定义簇的邻近度为取自两个不同簇的所有点对邻近度的平均值。


####  [Affinity Propagation](https://github.com/GGiecold/Concurrent_AP) 

 AP(Affinity Propagation)通常被翻译为近邻传播算法或者亲和力传播算法，是在2007年的Science杂志上提出的一种新的聚类算法。AP算法的基本思想是将全部数据点都当作潜在的聚类中心(称之为exemplar)，然后数据点两两之间连线构成一个网络(相似度矩阵)，再通过网络中各条边的消息(responsibility和availability)传递计算出各样本的聚类中心。

###  www.tfzoo.com

