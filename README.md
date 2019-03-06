# Toxic_Comment_Classification
- COMP6237 Data Mining Group coursework

1  Data Exploration

1.1  Check the basic info of the dataset

1.2  Class Imbalance

1.3  Multi-tagging

1.4  Wordclouds - Frequent words

2. Clean 
- 两个文件分别是两种清理方法后的评论内容，合并了训练集（前159571行）和测试集（后153164行）。
- ntlkl后缀名的是返回的是评论清洗后的内容，gensim后缀名返回的是每个评论提取的bigrams(二元词组)的list列表（这个是用于提取Topic(主题)的）
- 后面要做的三种模型，Naive Bayes SVM本身第二个核后面就有， LSTM 和 Logistic Regression 的核也都是用nltk包的TfidfVectorizer 分词的，只是用的参数不一样。