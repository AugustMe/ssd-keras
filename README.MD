# ssd-keras

## 主环境

tensorflow-gpu==1.13.1  
keras==2.1.5

## 训练自己的数据集

1. 修改 modei_data 文件夹中voc_classes.txt中的类别，将预训练权重放入model_data 文件夹中，如果不需要预训练权重的，将train.py中相应代码注释掉

2. 修改voc_annotation.py中的classes，改成数据集对应的类别

3. 修改train/train-multi-gpu.py[多GPU训练]中NUM_CLASSES


训练所需的ssd_weights.h5可以在百度云下载。  
链接: https://pan.baidu.com/s/17diCwawNy9WcqXhddl8qIw  
提取码: kquc  

## 测试模型

1. 修改ssd.py中model_path和classes_path
2. python get_dr_txt.py、 python get_gt_txt.py、 python get_map.py

## 参考

https://github.com/bubbliiiing/ssd-keras
