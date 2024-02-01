# 工程日志
## 项目
1、数据集采集

2、模型选择

3、模型训练

## 文件说明
/Data 储存爬取的数据集

/data_get 数据集爬取

  _/Try_Get_More.ipynb 二次数据爬取

/model_train 训练模型

/study 学习他人的文件

## 每日记录
2024 01 13 陈佳天 李杰瑞

- 10：30-11：00 完成课题申报意向表

- 11：11
  - 问题：如何同步代码?
  - 解决方法：学习使用Github和vsc同步  12：04但是失败了
- 12：05于是，我们使用了U盘复制这一高效的方法
- 13：18我们成功爬取了一些表情包（26张），并做到了只爬取jpg
- 13：22 data_get.ipynb为对于'https://www.doutub.com/'的爬取
        data_get2.ipynb 为对于'https://qq.yh31.com/zjbq/'的爬取（学习自csdn）
		data_get3.ipynb 为对于'https://www.dbbqb.com/'的爬取，但好像遇到了阻力（可能这个网站有反爬机制）
- 14：06 经过对data_get2.ipynb的改进对网页进行了多页爬取，暂未成功，可以爬几页
- 13：15 改进为data_get2_2.ipynb 分页进行爬取
- 15：36 爬取258张（257）

2024 01 17 
- 13 :04 决定以CNN作为深度学习的模型，并开始相应的模型原理学习
- 16：44初步完成了CNN的第一部分测试，建造了3units conv + max pooling的简单模型，打下了理论基础。作用是  ljr熟练了基于tensoflow的CNN编写  。 
- 16：44 更新爬取方式（未进行什么内容）

2024 01 22
- 14:43 整理文件
- 15:48 将尝试写在了/Keras_first_try中
- 16:13 在导入图片时失败
- 16:25 发现jpg如果为动图则无法导入
- 17:37 无法储存，开摆

2024 01 24
- 20:34 开始赶进度
- 20:42 解决无法储存问题
- 21:07 数据集单个过大，无法训练模型
- 21:26 发现好像不是数据集问题，而是穿入形式不对
- 21:56 依然没有解决
- 22:12 依然没有解决，放弃

2024 01 25
- 17:10 继续尝试
- 17:17 发现好像要把每一个数据改为相同大小
- 17:51 成功训练
- 18:05 发现由于数据不成比例，所以训练结果为全部判断为非攻击性



2024 01 26
- 20:10 为了解决数据不成比例的问题，随机上网爬取新的数据
- 21:00 遇到了问题并为此耗费40分钟，python报错是“url不正确”，此问题有待解决

2024 02 01
- 13:57 同步李杰瑞代码
- 15:47 完成爬取编写
- 17:19 爬了5页，共665张