# tech-doc

## Spark 

### Summary
Apache Spark 是专为大规模数据处理而设计的快速通用的计算引擎。
Spark是UC Berkeley AMP lab (加州大学伯克利分校的AMP实验室)所开源的类Hadoop MapReduce的通用并行框架，Spark，拥有Hadoop MapReduce所具有的优点；`但不同于MapReduce的是——Job中间输出结果可以保存在内存中，从而不再需要读写HDFS，因此Spark能更好地适用于数据挖掘与机器学习等需要迭代的MapReduce的算法`。<br>
Spark 是一种与 Hadoop 相似的开源集群计算环境，但是两者之间还存在一些不同之处，这些有用的不同之处使 Spark 在某些工作负载方面表现得更加优越，换句话说，Spark 启用了内存分布数据集，除了能够提供交互式查询外，它还可以优化迭代工作负载。

Apachespark 是一个用于大规模数据处理的统一分析引擎。它提供了 Java、 Scala、 Python 和 r 的高级 api，以及支持通用执行图的优化引擎。它还支持一组丰富的高级工具，包括 SQL 和结构化数据处理的 Spark SQL、机器学习的 MLlib、图形处理的 GraphX 以及增量计算和流处理的结构化流。

### Release note
在 Spark 2.0之前，Spark 的主要编程接口是弹性分布式数据集(Resilient Distributed Dataset，RDD)。在 Spark 2.0之后，RDDs 被 Dataset 替换，Dataset 与 RDD 一样是强类型的，但是在引擎盖下有更丰富的优化。仍然支持 RDD 接口，您可以在 RDD 编程指南中获得更详细的参考。但是，我们强烈建议您切换到使用 Dataset，它比 RDD 具有更好的性能。请参阅 SQL 编程指南以获取有关 Dataset 的更多信息 -- from offical doc.
