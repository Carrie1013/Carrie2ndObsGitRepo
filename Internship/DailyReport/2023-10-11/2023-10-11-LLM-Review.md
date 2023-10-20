- 除了GPT之外，可以用于词汇概括的语言模型方法：
	1. **BERT & Word2Vec & FastText**：
		1. BERT的嵌入来计算词汇的向量表示和平均向量表示，用表示来找到最相似的概括词
		2. BERT嵌入计算词汇向量表示和平均向量表示，predefine的一个vocabulary词汇表中找到最相似的词汇
	2. **TF-IDF & LSA (Latent Semantic Analysis)**：基于统计的方法以用于提取文本中的关键信息，从而生成概括性描述
	3. **Auto-encoders**：
		1. 自编码器训练为压缩和解压缩文本的表示
		2. 使用编码器部分生成文本的压缩表示，然后使用这些表示进行概括
	4. **T5 (Text-to-Text Transfer Transformer)**：
		 1. 多任务转换模型，可以用于各种文本到文本的任务，包括摘要和概括
	5. **Pointer-Generator Networks**：
		 1. 用于摘要的神经网络模型，结合了抽取式和生成式摘要的优点
	6. **Universal Sentence Encoder**：
		 1. Google的模型，为整个句子生成嵌入，而不仅仅是单个词汇
		 2. 同样的原理思路这些嵌入可以用于概括任务

- 无监督聚类方法：
	1. K-means
	2. DBSCAN(Density-Based Spatial Clustering of Applications with Noise)：
		- 基于密度的聚类方法，不需要提前指定簇的数量。
		- 可以发现任意形状的簇，对噪声点有良好的鲁棒性。
	3. GMM(Gaussian Mixture Model)：
		- 假设数据是由多个高斯分布生成的。
		- 使用期望最大化 (EM) 算法进行估计。
		- 可以捕获椭圆形簇。
	4. 层次聚类 (Hierarchical Clustering):
		- 建立一个层次分解的簇。
		- 不需要提前确定簇的数量。
		- 结果可以通过树状图 (dendrogram) 来表示。
	5. Agglomerative Clustering:
		- 一种自底向上的方法，开始时每个数据点都是一个簇，然后逐渐合并。
	6. 谱聚类 (Spectral Clustering):
		- 基于数据的相似性矩阵，使用图论方法。
		- 能够捕获复杂形状的簇，并且可以用于非凸集合的聚类。
	7. OPTICS (Ordering Points To Identify the Clustering Structure):
		- 类似于 DBSCAN，但可以处理不同密度的簇。
	8. **Mean Shift**:    
		- 不假设任何先验的簇形状。
		- 基于数据点的密度进行聚类。
	9. **Affinity Propagation**:    
	    - 通过将所有数据点都视为潜在的 exemplars 来进行聚类。
	    - 不需要预先设定簇的数量。

