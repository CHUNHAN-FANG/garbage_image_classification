# 图识垃圾
#### 基于DenseNet的迁移学习实践，实现生活垃圾图像分类

图识垃圾是大学时期（2019）实践的科创项目，上海2019年7月开始全面执性垃圾分类（干垃圾、湿垃圾、可回收垃圾、有毒有害垃圾），故响应政策，结合图像分类技术，训练了生活垃圾图像分类模型，并制作了垃圾分类智能助手微信小程序。<br>
该项目大量调研生活垃圾分类规定（收集六千余条生活垃圾细目），并结合垃圾图像视觉规律，对主要生活垃圾拟定图像分类方案。原项目列出3种方案（覆盖90%左右生活垃圾），如下：
<br><img width="500" alt="垃圾分类方案" src="https://user-images.githubusercontent.com/48016042/167675737-c2f5e647-e526-4306-9384-5b87725d0b10.png">

本项目代码中以方案C（16综合大类）为例，实现图像样本处理、搭建浅层CNN、利用现有深度卷积DenseNet迁移学习。
* 01 [图像样本集处理](https://nbviewer.org/github/CHUNHAN-FANG/garbage_image_classification/blob/main/01图像样本集处理.ipynb)

* 02 [GC_modelC_CNN](https://nbviewer.org/github/CHUNHAN-FANG/garbage_image_classification/blob/main/02GC_modelC_CNN.ipynb)
<br>搭建的CNN架构如下：
<br><img width="500" alt="CNN架构" src="https://user-images.githubusercontent.com/48016042/167677811-86ec18ed-8d5c-4b29-bf25-345a6a5654b3.PNG">

* 03 [GC_modelC_TR_DenseNet201](https://nbviewer.org/github/CHUNHAN-FANG/garbage_image_classification/blob/main/03GC_modelC_TR_DenseNet201.ipynb)
<br>迁移学习示意如下：
<br><img width="400" alt="迁移学习结构" src="https://user-images.githubusercontent.com/48016042/167677374-46e06a3e-ab5b-476f-8909-1082fd321b9f.PNG"><img width="300" alt="迁移学习模型架构" src="https://user-images.githubusercontent.com/48016042/167677418-5929e604-9abd-456c-b392-fd8732f05022.PNG">

* [图识垃圾小论文]
<br><br>
另外，图识垃圾微信小程序（科创项目demo）如下，可提供文本、语音、图像查询生活垃圾分类，用户交互界面显示的垃圾细分条目由百度识图（通用场景及物体识别）API提供技术辅助，另外本项目训练的modelC生活垃圾图像分类模型也上载在微信小程序云端，同步调用实现双保险。
<br><img width="160" alt="图识垃圾小程序二维码"  src="https://user-images.githubusercontent.com/48016042/167683191-18878366-75b1-4d57-9ea0-3e9ad41e02ce.png">
<br><br>
注：以上代码仅为项目部分实践记录，及零散学习笔记，欢迎指正
