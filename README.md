
## CardiacAI

See https://arxiv.org/abs/1808.08277.pdf

Also see my [website page](https://www.cmwonderland.com/blog/2018/08/16/95_medical_image_project/)

## Goal and Philosophy

  Diagnosis of cardiac diseases using AI
  We are trting to use the deep learning technique to diagnose cardiac disease.

## Data source

  The X-ray images we collected are from two hospitals in Nanyang, Henan and a foreign dataset from Indiana University
 [openichestdataset](https://openi.nlm.nih.gov/gridquery.php?q=&coll=cxr)

<img src="https://github.com/cardiacai/cardiacai/raw/master/images/%E5%9B%BE%E7%89%87%E9%A2%84%E5%A4%84%E7%90%86%E6%B5%81%E7%A8%8B.png" width = "600" height = "500" alt="" align=center />

  

## Why CardiacAI

  

## Requirements

   ```python = 2.7```
   <br>```keras >= 2.0.4```
   <br>```opencv >= 2.4```

## documentation

  
##### 主要代码解释：
     在[bin](https://github.com/cardiacai/CardiacAI/tree/master/bin)和[preprocess](https://github.com/cardiacai/CardiacAI/tree/master/preprocess)文件夹下的是我们的主要代码,[iamges](https://github.com/cardiacai/CardiacAI/tree/master/images)下面有我们的一些结果与分析的示例等。[results](https://github.com/cardiacai/CardiacAI/tree/master/results) 下有一些结果。由于我们在多种数据集上使用多个模型进行了训练、预测和分割以及多种分析，为避免内容杂乱，并没有上传详细的结果和图片。
  
##### 一些可能产生疑问的脚本的解释
   <br>  bin/analyze.py脚本使用梯度算法做了图像的sensitivity analysis，来分析图像学习到的特征，bin/lrp.py则使用了deep taylor decomposition的可视化方法来分析特征。<br/>
   <br>  bin/extract_dicom、bin/preprocess、bin/remove_sensitive_info_dicom.py和preprocess文件夹下的多个脚本则完成了一系列的预处理工作，包括去除，转换图像格式，调整大小和分辨率、二值化、进行轮廓提取和多边形拟合、将traces转化为mask等操作。<br/>
   <br>  bin/models则定义了多个深度学习模型，包括VGG16、U-net以及卷积层由VGG16代替的U-net网络。<br/>
## How It Works

## Credits 
Binbin Shi, Kewen Wang, Xupeng Chen

## Work Logs


---

#### Contact
xp-chen14@mails.tsinghua.edu.cn

