# Toxic_Comment_Classification
COMP6237 Data Mining Group coursework
Naive Bayes：
Naive Bayes is one of the most effective data mining algorithms for machine learning and inductive learning. The structural basis of the naive Bayes classifier is a classification method based on Bayes' theorem and feature condition independent hypothesis, which is different from the model based on the linear hypothesis (linear classifier and support vector machine classifier). Naïve Bayes has a wide range of practical applications, especially in the task of text categorization, including the classification of news and the screening of spam. Because the number of tasks in our group processes texts data, and a typical feature of text data is that its dimensions are large, such as a document, there will be thousands or even tens of thousands of words, but the vocabulary difference between documents of different types of topics is larger. Instead of considering the order in which words appear, the bag of words model is assumed, assuming that the appearance of each word in the text is independent. Text classification problems based on such assumptions can be solved using the naive Bayesian method. The simplicity of Naive Bayes is reflected in the assumption of the independence of each feature, and the independence hypothesis, which greatly reduces the parameter hypothesis space, and its learning and prediction is greatly simplified. Although the conditional independence assumption is simple, the classification effect of the naive Bayes classifier is still good, even if there is a strong correlation between the features.

朴素贝叶斯是最有效的用于机器学习和归纳学习的数据挖掘算法之一。朴素贝叶斯分类器的构造基础是基于贝叶斯定理与特征条件独立假设的分类方法，与基于线性假设的模型（线性分类器和支持向量机分类器）不同。朴素贝叶斯有着广泛的实际应用环境，特别是在文本分类的任务中，包括新闻的分类，垃圾邮件的筛选。因为我们小组的任务数处理文本数据，而文本数据的一个典型特征就是其维度较大，比如一篇文档，会有几千甚至上万个词，但是不同类型或主题的文档所用词汇差距较大，可以不考虑词汇出现的顺序，即采用bag of words模型，假设文本中每个词的出现都是独立的。基于此类假设的文本分类问题，可以采用朴素贝叶斯方法进行求解。朴素贝叶斯的朴素体现在对各个特征的独立性假设，加上独立性假设后，大大减少了参数假设空间，其学习与预测大为简化。尽管条件独立性假设很朴素，但是朴素贝叶斯分类器的分类效果依然很好，即使各特征之间存在较强的相关性。


## 结果统计

|组合|Accuracy|Val_Accuracy|提交结果score|
|---|--------|------------|------------|
|raw_comment|0.9816|0.9987|0.96730|
|raw_comment + random under-sampling|0.9302|0.9755|0.97720|
|clean_comment|0.9819|0.9986|0.9674|
|clean_comment + random under-sampling|0.9336|0.9746|0.9632|
