# 图识垃圾
基于DenseNet的迁移学习实践，实现生活垃圾图像分类

该项目是大学时期（2019）实践的，上海2019年7月开始全面执性垃圾分类，故响应政策，项目大量调研生活垃圾分类规定（收集六千余条生活垃圾细目），并结合垃圾图像视觉规律，对主要生活垃圾拟定图像分类方案。原项目列出3种方案（覆盖90%左右生活垃圾），如下：
<br><img width="500" alt="垃圾分类方案" src="https://user-images.githubusercontent.com/48016042/167675737-c2f5e647-e526-4306-9384-5b87725d0b10.png">

本项目代码中以方案C（16综合大类）为例，实现图像样本处理、搭建浅层CNN、利用现有深度卷积DenseNet迁移学习。
* 01 图像样本集处理：https://nbviewer.org/github/CHUNHAN-FANG/garbage_image_classification/blob/main/01图像样本集处理.ipynb
* 02 GC_modelC_CNN：https://nbviewer.org/github/CHUNHAN-FANG/garbage_image_classification/blob/main/02GC_modelC_CNN.ipynb
<br>搭建的CNN架构如下：
<br><img width="500" alt="CNN架构" src="https://user-images.githubusercontent.com/48016042/167677811-86ec18ed-8d5c-4b29-bf25-345a6a5654b3.PNG">
* 03 GC_modelC_TR_DenseNet201：https://nbviewer.org/github/CHUNHAN-FANG/garbage_image_classification/blob/main/03GC_modelC_TR_DenseNet201.ipynb
<br>迁移学习示意如下：
<br><img width="400" alt="迁移学习结构" src="https://user-images.githubusercontent.com/48016042/167677374-46e06a3e-ab5b-476f-8909-1082fd321b9f.PNG"><img width="300" alt="迁移学习模型架构" src="https://user-images.githubusercontent.com/48016042/167677418-5929e604-9abd-456c-b392-fd8732f05022.PNG">
* 图识垃圾小论文：https://s3.us-west-2.amazonaws.com/secure.notion-static.com/81a49660-b12c-405e-923f-0dfc0d16f167/%E6%96%B9%E7%BA%AF%E6%B6%B5_%E5%9B%BE%E8%AF%86%E5%9E%83%E5%9C%BE%EF%BC%9A%E5%9F%BA%E4%BA%8E%E8%BF%81%E7%A7%BB%E5%AD%A6%E4%B9%A0%E7%9A%84%E5%9B%BE%E5%83%8F%E8%AF%86%E5%88%AB%E5%AE%9E%E8%AF%81%E7%A0%94%E7%A9%B6.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220510%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220510T160845Z&X-Amz-Expires=86400&X-Amz-Signature=dbbb6edef7a064f9b82b5ef49d1feddf24a760336f0a2524d41212d8e78e09ba&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22%25E6%2596%25B9%25E7%25BA%25AF%25E6%25B6%25B5_%25E5%259B%25BE%25E8%25AF%2586%25E5%259E%2583%25E5%259C%25BE%25EF%25BC%259A%25E5%259F%25BA%25E4%25BA%258E%25E8%25BF%2581%25E7%25A7%25BB%25E5%25AD%25A6%25E4%25B9%25A0%25E7%259A%2584%25E5%259B%25BE%25E5%2583%258F%25E8%25AF%2586%25E5%2588%25AB%25E5%25AE%259E%25E8%25AF%2581%25E7%25A0%2594%25E7%25A9%25B6.pdf%22&x-id=GetObject

注：以上代码仅为项目部分实践记录，及零散学习笔记，欢迎指正
