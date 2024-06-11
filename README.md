# **CCAC2024结合用户画像信息中文情绪分类评测**

## 背景介绍

在本届大会中，我们将举办“结合用户画像信息中文情绪分类”评测项目。情绪分类是一项关键的情感分析任务，其在学术界和工业界都引起了广泛关注。在社交媒体、在线评论、产品反馈等各类文本中，有效地识别和分类用户的情绪，对于提升产品服务、优化用户体验等方面具有重大价值。目前，虽然存在许多关于情绪分类的任务和数据集，但是大多数都仅仅关注于单一的文本内容，忽视了用户画像信息的重要性。用户画像信息，如用户的昵称、地区等，往往能够提供更丰富的上下文信息，帮助更准确地理解和识别用户的情绪。尤其在面临ChatGPT等大模型冲击的背景下，如何利用这些丰富的用户画像信息，提高情绪分类的效果，成为了一个具有挑战性的问题。因此，我们标注了一个结合用户画像信息的情绪分类数据集，该数据集包括用户的昵称、地区、性别、好友等要素，支持对隐式情绪的识别和理解。我们基于该数据，设定了结合用户画像信息中文情绪分类评测任务。

本届评测由中国中文信息学会情感计算专委会（CIPS-CCAC）主办，江西财经大学承办，诚挚欢迎各界人士参与。



## 评测内容

本届大会中，我们将举办“结合用户画像信息中文情绪分类”评测项目，在比赛中我们提供了一个结合用户画像信息的情绪分类数据集作为评测语料。

数据集：我们从新浪微博网站上收集了用户的信息，由专业标注员进行了中文情绪分类的标注，整理为txt格式的文件。

以下是详细任务介绍。

**结合用户画像信息中文情绪分类**

​	给定一个用户画像（包括用户所在的地区、性别、关注人列表、发表的历史文本等）以及一个用户文本，参赛模型需判断用户文本所表达的情绪，输出的情绪是下面五种情绪之一：喜、哀、惊、恐、怒。



**数据样例：**

输入：

**用户画像**

- ​	地区：上海
- ​	性别：女
- ​	关注的人列表：...
- ​	用户发表的历史文本列表：...

**需要判断情绪的文本**

​	刚刚买的新裙子，真的超级好看，我简直爱死了！

输出：喜

--------------------------------------------------------------------------

输入：

 **用户画像**

- 地区：北京
- 性别：男
- 关注的人列表：...
- 用户发表的历史文本列表：...

**需要判断情绪的文本**

​	我心爱的球队又输了，真是太让人失望了。

输出：哀

--------------------------------------------------------------------------

评价指标： Macro-F1 score

$$
F1_{macro}=\frac{1}{N} \sum_{i=1}^{N} F1_{i}
$$

其中， $N$是类别数量，
$F1_{i}$ 是第i类的F1分数

$$
F1_{i}=2\times \frac{Precision_{i}\times Recall_{i}}{Precision_{i}+Recall_{i}}
$$

$$
Precision_i=\frac{TP_i}{TP_i+FP_i}
$$

$$
Recall_i=\frac{TP_i}{TP_i+FN_i}
$$

其中，
$Precision_i$是模型预测为第i类的样本中实际为第i类的比例，
$Recall_i$是实际为第i类的样本中被模型预测为第i类的比例。



## 报名网站
[报名表](https://docs.qq.com/form/page/DY1BmR1JWUVZneFpB)


## 提交方式
请参赛团队将最终的预测结果发送到qiangminjie27@gmail.com，在邮件中请注明机构名称以及负责人姓名。

注意：如果多次重复发送的话，以最新一次为准。



## 重要日期

| 事项                       | 时间          |
| -------------------------- | ------------- |
| 任务发布与报名启动         | 2024年4月20日 |
| 训练集语料发布             | 2024年4月30日 |
| 测试集语料发布             | 2024年6月12日 |
| 提交截止（报名结束）       | 2024年6月15日 |
| 比赛结果公布               | 2024年6月22日 |
| CCAC2024大会召开及颁奖典礼 | 2024年6月30日 |



## 联系方式

如有疑问，请致信评测会务组：王中卿 wangzq@suda.edu.cn、强敏杰 qiangminjie27@gmail.com



## 致谢

主办方：中国中文信息学会情感计算专委会（CIPS-CCAC）

承办方：江西财经大学
