## RFM模型及用例实践##


RFM（Recency，Frequency，Monetary）分析是一种营收市场技术，主要是通过分析付费用户的行为，对付费用户进行分层，从而达到精准营销的目的。有兴趣可参考 : RFM模型_wiki。RFM的变体 RFD（Recency，Frequency，Duration）也可用与于对网站用户的其他行为分析，详情及其他变体不在此赘述。

【参数解释】

R：最近一次消费距今天数(Recency)
F： 消费频率(Frequency)
M：消费金额(Monetary)
【前提假设】

最近购买产品的用户更容易产生下一次消费行为
消费频次高的用户，用户满意度高，忠诚度高，更容易产生下一次消费行为
消费金额高的用户更容易带来高消费行为
具有相同RFM_value  的用户有相似的市场行为
【数据挖掘&数据化运营】

这里主要介绍RFM模型在网站营收付费用户的应用（Case Study），主要分为以下几个步骤：
Step1，RFM 分析和付费用户分层（cluster）
Step2，跟踪用户在不同状态的转移 （classification）
Step3，付费用户的产品推荐（association rule）（有可能不做，因为产品较少且产品相似度较高）


数据挖掘中的多元分类机器学习方法，主要尝试了Naive Bayes，k-近邻(KNN)，决策树，随机森林，神经网络等方法，其中预测准确率比较高的是随机森林，神经网络和决策树，这里欲采取决策树方法，主要原因：（1）通过调参可以达到和随机森林及神经网络差不多的准确率ACC；（2）AUC值相对比较高；（3）结果可解释性比较强。
【附】多元分类器的性能比较

![image](https://user-images.githubusercontent.com/39177230/131254616-a28a07bc-74b7-4fe3-8aa5-d331008b3a99.png)

Reference：
[RFM模型及其用户运营实践](https://blog.csdn.net/yeonki/article/details/50573235)




















