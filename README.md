
## CardiacAI
  欢迎访问我们的网站<br/>
  [VISIT OUR WEBSITE：CardiacAI](http://cardiacai.cn)

## Goal and Philosophy

  Diagnosis of cardiac diseases using AI
  We are trting to use the deep learning technique to diagnose cardiac disease.

## Data source

  The X-ray images we collected are from two hospitals in Nanyang, Henan and a foreign dataset from Indiana University
 [openichestdataset](https://openi.nlm.nih.gov/gridquery.php?q=&coll=cxr)

<img src="https://github.com/cardiacai/cardiacai/raw/master/images/%E5%9B%BE%E7%89%87%E9%A2%84%E5%A4%84%E7%90%86%E6%B5%81%E7%A8%8B.png" width = "600" height = "500" alt="" align=center />

  

## Why CardiacAI
  Your are welcome to read the stories on our website.
  [为什么是心脏病](http://www.cardiacai.cn/why)
  

## Requirements

   ```python = 2.7```
   <br>```keras >= 2.0.4```
   <br>```opencv >= 2.4```

## documentation
  [技术文档](http://www.cardiacai.cn/techlog)
  
##### 主要代码解释：
     在[bin](https://github.com/cardiacai/CardiacAI/tree/master/bin)和[preprocess](https://github.com/cardiacai/CardiacAI/tree/master/preprocess)文件夹下的是我们的主要代码,[iamges](https://github.com/cardiacai/CardiacAI/tree/master/images)下面有我们的一些结果与分析的示例等。[results](https://github.com/cardiacai/CardiacAI/tree/master/results) 下有一些结果。由于我们在多种数据集上使用多个模型进行了训练、预测和分割以及多种分析，为避免内容杂乱，并没有上传详细的结果和图片。
  
##### 一些可能产生疑问的脚本的解释
   <br>  bin/analyze.py脚本使用梯度算法做了图像的sensitivity analysis，来分析图像学习到的特征，bin/lrp.py则使用了deep taylor decomposition的可视化方法来分析特征。<br/>
   <br>  bin/extract_dicom、bin/preprocess、bin/remove_sensitive_info_dicom.py和preprocess文件夹下的多个脚本则完成了一系列的预处理工作，包括去除，转换图像格式，调整大小和分辨率、二值化、进行轮廓提取和多边形拟合、将traces转化为mask等操作。<br/>
   <br>  bin/models则定义了多个深度学习模型，包括VGG16、U-net以及卷积层由VGG16代替的U-net网络。<br/>
## How It Works
  [原理介绍](http://www.cardiacai.cn/dlmodel)<br/>
  
<br>总体流程
 <img src="https://github.com/cardiacai/CardiacAI/raw/master/images/pipeline.png" width = "600" height = "500" alt="" align=center />
 <br/>
 <br/>
 <br>深度学习流程
   <img src="https://github.com/cardiacai/CardiacAI/raw/master/images/%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E9%83%A8%E5%88%86%E6%B5%81%E7%A8%8B.png" width = "400" height = "500" alt="" align=center />
  <br/>
  <br/>
 <br>VGG
  <img src="https://github.com/cardiacai/CardiacAI/raw/master/images/%E6%88%91%E4%BB%AC%E7%9A%84VGG%E6%A8%A1%E5%9E%8B.png" width = "200" height = "500" alt="" align=center />
 <br/>
 <br/>
 <br>VGG-U-net 
  <img src="https://github.com/cardiacai/CardiacAI/raw/master/images/%E6%88%91%E4%BB%AC%E7%9A%84VGG%2BU-net%E6%A8%A1%E5%9E%8B.png" width = "600" height = "500" alt="" align=center />
  <br/>
   <br>RNN-CNN
  <img src="https://github.com/cardiacai/CardiacAI/raw/master/images/RNN-CNN.png" width = "600" height = "500" alt="" align=center />
  <br/>

## Credits 
  [枕叶纺者们](http://www.cardiacai.cn/aboutus)
###### 史斌斌
   本科毕业于清华大学生命学院，现清华大学生命学院博士三年级，专业方向为生物信息学。
###### 王炣文
   北京邮电大学网络工程专业本科三年级。
###### 陈旭鹏
   清华大学生命学院本科二年级。

## Work Logs
  [工作日志](http://www.cardiacai.cn/worklog)





---

#### 您可以通过以下方式联系到我们：
- 网站 [CardiacAI](http://cardiacai.cn)
- 邮箱 240682348@qq.com

