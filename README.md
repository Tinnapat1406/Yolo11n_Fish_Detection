# Yolo11n_Fish_Detection

**Note :** File is large to display on GitHub if you want to see my practice work. *Please download raw file*

### **Implement**
This Practice is train a YOLO11n model on a custom COCO fish dataset on Colab Notebook.

## **Library**
![Numpyt](https://img.shields.io/badge/-Numpy-013243?&logo=NumPy)

![matplotlib](https://camo.githubusercontent.com/9af8ba2f016bf42126b61646d5df7264115cadfd4a8be0073aa812a2107e94f2/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4d6174706c6f746c69622d2532333146343235462e7376673f267374796c653d666f722d7468652d6261646765266c6f676f3d6d6174706c6f746c6962266c6f676f436f6c6f723d7768697465)

**Ultralytic**

![cv2](https://img.shields.io/badge/OpenCV-27338e?style=for-the-badge&logo=OpenCV&logoColor=white)


**Dataset** : 
```
https://universe.roboflow.com/agwel/fish-fry-r5wy2-5wp79/dataset/1
```

Install Library 
```
!pip install ultralytics
import numpy as np
import matplotlib.pyplot as plt
from ultralytics import YOLO
import cv2
from google.colab import files
import io
from PIL import Image
from skimage import data
import yaml
import os
```

<img width="980" height="305" alt="image" src="https://github.com/user-attachments/assets/b8a72316-f66b-4187-8042-d4e35684c322" />

training the YOLO11n model on your custom dataset using the configuration file, ensuring the dataset paths are correct.
```
!rm /content/custom_data/train/labels.cache
!yolo detect train data=/content/custom_data/data.yaml model=yolo11n.pt epochs=50
```
### Result with Test Dataset 

<img width="1536" height="2048" alt="image" src="https://github.com/user-attachments/assets/165a9b30-044b-4088-9fef-fef928dd75ec" />

## Metric
<img width="599" height="298" alt="image" src="https://github.com/user-attachments/assets/615f3b4a-29ce-4ec0-8556-5c3db1a7e3ad" />

**Reference** : https://colab.research.google.com/github/EdjeElectronics/Train-and-Deploy-YOLO-Models/blob/main/Train_YOLO_Models.ipynb 
