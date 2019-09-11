# Data_Analysis_Projects
这里包含几个职业培训期间做的项目，每个项目都对应着一个子目录，其中包括一个脚本文件和一个html文件，有些子目录还有项目相关的数据集。以下是项目相关的介绍：
## Project1:探索美国共享单车数据
数据来自美国共享单车系统Motivate。原始数据保存在三个csv文件中，分别对应芝加哥、华盛顿、纽约三个城市的共享单车数据。    
三个数据文件都包括核心的6列：    
* 起始时间 Start Time
* 结束时间 End Time
* 骑行时长 Trip Duration
* 起始车站 Start Station
* 结束车站 End Station
* 用户类型 User Type    

芝加哥和纽约市文件还包含以下两列：   
* 性别 Gender
* 出生年份 Birth Year     

这个项目使用Pandas的DataFrame数据结构处理来自csv文件的数据，程序首先向用户询问他们想要了解的单车信息，然后从数据集中筛选出相应的数据，有一定的交互，并且通过流程控制提高了对用户输入的容错能力。

## Project2:探索电影数据集
数据来源为“电影数据库”（TMDb，The Movie Database），包含 1 万条电影信息，包括用户评分和票房。数据同样保存在csv文件中。     
本项目旨在理清数据分析的各个流程(提出问题->收集、评估、清理数据->探索性数据分析->得出结论->传达结论)，及综合使用Python的Numpy、Pandas处理数据，和使用Matplotlib完成可视化。项目首先会提出问题，然后对数据集进行适当清理，通过分析之后完成可视化并给出结论。

## Project3:分析商业网站A/B测试结果
本项目数据集来自一个电商网站 A/B 测试结果，包含控制/实验组、用户是否转化等信息。我们需要根据这些数据给出网站使用新版本 or 旧版本页面的建议。

项目过程：
* 对数据进行简单的清洗，计算控制组和实验组的转化率；
* 构造假设检验，检验新旧页面的转化率之差是否为 0。采取 Boostrap 模拟和 z 检验两种方案实现；
* 构造逻辑回归模型，以页面类型为自变量预测用户转化，并将其结果和假设检验的结果进行比较；
* 构造逻辑回归模型，以页面类型和用户所在国家为自变量预测用户转化（考虑页面类型和用户所在国家之间的交互作用），并解释模型输出；
* 根据以上步骤，对业务部门给出建议：继续使用旧页面，还是更换新页面？又或是延长测试期？
* 掌握假设检验及逻辑回归的 Python 实现。

## Project4:狗狗数据清洗
本项目旨在在满足数据整洁度定义（每个变量形成一列、每组观测形成一行、没类数据形成一个表）的情况下，将数据汇总在一起。最终对数据进行简易分析，并产出可视化。本项目需要用到三个相关数据集：twwiter API 获取的 json 数据、包含点赞数的附加 csv 数据、狗狗种类预测 csv 数据。主要借助工具为 Python、pandas、Matplotlib等。

## Project5:葡萄酒数据集的探索性数据分析
探索性数据分析是数据建模前重要的一步，借助这个过程可以更深入地理解数据，及探索变量间潜在的关系，为正式建模做准备。其核心工具为 R 和 ggplot2 包，通过 ggplot2 强大的图层语法，可以快速、清晰地实现可视化。本项目涉及一个接近4900组观测、12个变量的白葡萄酒数据集。为理解葡萄酒的众多特征与专家评分的关系，我将根据单变量-双变量-多变量的脉络对数据进行探索：在单变量分析中，绘制每个变量的直方图或条形图，以理解每个变量的分布情况、有无异常值等；在双变量分析中，对感兴趣的成对变量绘制散点图、盒须图等，研究变量之间的相关性；在多变量分析中，进一步引入第三个变量，研究多个变量之间的交互关系。
