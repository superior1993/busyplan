***Week 43 of 2017***

**The ONE thing** : 

### 24.10 Tue
**Tomorrow TODO**

**Reflection**

**Summary**


### 25.10 Tue
**Tomorrow TODO**

- 继续关于深度的研究，找数据集，确认点云转换
- 跟进GAN道路生成的研究

**Reflection**

- vkitti数据集的深度是由z-buffer生成，直接存储深度z。前方有遮挡的情况下z-buffer会将后面的信息hidden。近处深度预测较好，远处深度误差较大。我们的3Dreconstruction近距离曲面话的问题可能是由于近处估值太近，调整y轴有所改善。深度预测方法还有w-buffer。因为并非真实世界深度图，暂时不继续研究。

**Summary**

- 盛大孵化器
- 断网期间复习了下numpy (⊙﹏⊙)b
- 看了下vkitti深度估算方法z-buffer
- 寻找合适数据集，暂定kitti
	- 弯道明显/路的界限清晰
	- 尽量没有车辆等过于复杂的干扰（我的考虑）
- 今日网络情况堪忧


### 24.10 Tue
**Tomorrow TODO**

- 根据讨论结果，全力帮助本周GAN的目标，生成看得过去的路的图片
- 如果GAN的研究不需要帮忙，稳步推进对深度预测的研究

**Summary**

- 讨论结果，为集中与GAN的研究设定目标和明确的停止标准以及停止后备案方法
- 下班前提起公司发展目标的讨论，让大家都跟着下班晚了 (⊙﹏⊙)b
- 量化结果显示63000次模型的数据评分较论文还是低，但考虑到使用的不是一个训练集，参考价值不大。考虑新训练模型选用论文中提到的kitti数据集，方便测评。
- 因为vkitti数据集自身表示方式的问题，讨论决定改用真实数据集训练模型，会涉及的问题：点云转换计算，坐标系变换
- 新测试模型因为存储器满了的原因暂停训练，模型保存的是epoch17or18 的参数，进行视觉测评，效果提升明显，修正了前一模型深度点散装延一个方向分布的问题
- 上午和zw讨论确认virtualkitti数据集深度为点到平面深度，3D reconstruction 会出现坡度问题。

日常：

- [x] 每天开始工作前阅读15min
- [ ] 工作前今日计划确认 晚睡早上目标明确没确认
- [x] 工作总结 回家后总结安排

+_+ 语气上好像又强人所难了，修行不够

### 23.10 Mon

**Schedule**

- [x] 确认色温显示方法
- ~~找到方法将3D点云信息导入rViz方便查看~~ zw找到pyntcloud Library 方便的实现
- 晚上到0点完成深度预测视觉测试的样本

早会： 9点前到office，周三、周六分享，日常集中手上项目，工作计划与工作总结

- [x] 今日工作，继续p2p深度预测，具体记录在github上[Issues 5](https://github.com/createamind/busyplan/issues/5)

反思：
图像处理技术需要加强，要更熟练。目前个人主要问题，各项技术都缺乏熟练度，解决方法，只学习一个框架（TensorFlow）多做练习，多请教同事。尽快提升到专业水平。

日常：

- [x] 每天开始工作前阅读15min
- [x] 工作前今日计划确认
- [x] 工作总结
