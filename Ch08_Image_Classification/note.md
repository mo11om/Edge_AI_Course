# 8.4.影像分類實作
Colab Open Model Zoo 影像分類範例
https://colab.research.google.com/drive/161C-TzrSdcLx5ePApaN0BkHlYygncmG6?usp=sharing
---
 


---
```
from pathlib import Path

import cv2 # 導入 OpenCV
import matplotlib.pyplot as plt
import numpy as np
import openvino as ov
### 
import os
os.environ['CUDA_VISIBLE_DEVICES'] = '-1'
import tensorflow as tf
###
# 下載`notebook_utils`模組
import urllib.request
urllib.request.urlretrieve(
    url='https://raw.githubusercontent.com/openvinotoolkit/openvino_notebooks/main/notebooks/utils/notebook_utils.py',
    filename='notebook_utils.py'
)

from notebook_utils import download_file # 導入 download_file 模組

import ipywidgets as widgets # 導入 ipywidgets 模組
```

##  指定輸入
- 資料排列方式為 "NHWC" 或 "NCHW" 在不同地方 不一樣
- 影像色彩通道順序為 "BGR"或 "RGB" 在不同地方`   不一樣
```
 
layout = "NHWC" # 指定輸入資料排列方式為 "NHWC" 或 "NCHW"
color_ch = "BGR" # 指令輸入影像色彩通道順序為 "BGR" 或 "RGB"
```