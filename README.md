# LULC-Classification-on-TALANDCOVER-Dataset
![ alt text ](https://img.shields.io/badge/license-MIT-green?style=&logo=)
![ alt text ](https://img.shields.io/badge/-Jupyter-F37626?logo=Jupyter&logoColor=white)
![ alt text ](https://img.shields.io/badge/-NumPy-013243?logo=Numpy&logoColor=white)
![ alt text ](https://img.shields.io/badge/-Google_Colab-F9AB00?logo=googlecolab&logoColor=white)
![ alt text ](https://img.shields.io/badge/-TensorFlow-FF6F00?logo=TensorFlow&logoColor=white)
![ alt text ](https://img.shields.io/badge/-Keras-D00000?logo=Keras&logoColor=white)

This repository presented an efficient deep learning model, named Mobile-UNet, for land cover classification, which is inspired by MobileNetV2 and U-Net. The model was evaluated on a public dataset (TALANDCOVER) in TIF format. Compared with U-Net, Mobile-UNet requires fewer parameters, and achieved high segmentation accuracy. In practical applications, the land cover in multiband imagery is mostly imbalanced and facing semantic issues, which makes the network difficult to train. In this case, vegetation classes exhibited significant similarities, leading to challenges in boundary delineation. To solve this problem, we utilize the improved loss function, focused on two most challenging classes, to make the model easier to train. The neural network's performance was evaluated with commonly used segmentation metrics. The model's architecture allowed us to observe the large learning capabilities on the data.

<img src='https://github.com/user-attachments/assets/40d9b5a5-dcb9-42a2-b995-203763675327' height='200'/>

<img src='https://github.com/user-attachments/assets/c1183c20-a693-47b5-a653-8e3c9b000802' width='450'/>

Evaluation metrics across each class:
| Label | Class         | Precision | Recall | F1-Score |  IoU  | Kappa |
|-------|---------------|-----------|--------|----------|-------|-------|
| 0     | Bare-Degraded | 0.7681    | 0.7900 | 0.7789   | 0.6379| 0.7505|
| 1     | Grassland     | 0.7170    | 0.5899 | 0.6472   | 0.4785| 0.5378|
| 2     | Agriculture   | 0.5493    | 0.7016 | 0.6162   | 0.4453| 0.4940|
| 3     | Forest        | 0.7814    | 0.7410 | 0.7607   | 0.6138| 0.7031|
| 4     | Water         | 0.8940    | 0.8605 | 0.8769   | 0.7808| 0.8652|
| 5     | Built-Up      | 0.8652    | 0.8457 | 0.8553   | 0.7472| 0.8354|

Aggregated performance metrics:

**Precision:** 0.762498<br>
**Recall   :** 0.754779<br>
**F1       :** 0.755873<br>
**IoU      :** 0.617237<br>
**Kappa    :** 0.697668<br>
