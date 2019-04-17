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
- 后面要做的三种模型，Naive Bayes SVM本身第二个核后面就有， LSTM 和 Logistic Regression 的核也都是用nltk包的TfidfVectorizer 分词的，只是用的参数不一样，后面认为需要统一为一样的。我用的TfidfVectorizer 分词的参数在我分支下的代码文件的Bigrams中。

04.16 Update:

pre的feedback已经更新：https://hackmd.io/KRmH_7ahQACARMqqRFAiJg?view

Data Exploration:
1. 添加了wordcloud的部分，由于加蒙版运行速度过慢，保持了普通的样式
2. wordcloud中重复的词可以设置去除（collocations=False）

Feature engineering:
1. 添加了leaky feature的部分
Corpus cleaning:
1. 词库用的是kernel中的Aphost lookup dict，可以再添加
2. clean时按照markus的建议没有全部转小写
