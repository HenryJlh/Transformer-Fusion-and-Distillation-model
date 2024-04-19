# Transformer-Fusion-and-Distillation-model
## Abstract
This paper shows the potential of ViT model (Vision Transformer) to achieve multi-modal fusion based on a case implementation of "cortical cataract intelligent grading". This project intends to learn pathological features that are in line with clinical judgment by multi-modal fusion of image and sub-label from local features. At the same time, a distillation network framework is proposed to eliminate the input of sub-label in the test, so that better classification results can be obtained by relying on images alone. 
## Methods
Firstly, Image features and text features (sub-label features) are extracted based on residual network (ResNet) and deep-learning neural network (DNN), respectively. 
Secondly, The multi-modal fusion of image and text features is realized by using ViT model framework.
Lastly, The trained high-precision fusion model is used to guide the learning of residual network through knowledge distillation to achieve no sublabel input and improve the accuracy of image unimodal. 
## Datasets (not public)
The dataset can be divided into two parts, image and text. There are 2050 cortical cataract images differeing in levels from 0-7. The higher level is, the more serious the cataract symptom is. 0 level means the eye is healthy without any signs of cortical cataract. The text dataset is sub-label data, which is mannually labeld and used to help doctors to judge the severity of the cataract symptom. Evey image corresponds to six sublables. And each sublabl describes one local feature of the image. 
## Results
Our high-precision fusion model achieves 93.02% accuracy on the cortical cataract dataset, and the residual network of knowledge distillation achieves 79.27% accuracy without sublabel input, which is nearly 5% higher than that of residual network alone.
![image](https://github.com/HenryJlh/Transformer-Fusion-and-Distillation-model/assets/106720714/87df2571-9a96-4846-b0d3-acffdf4675d3)
## 1. Features Extraction
![image](https://github.com/HenryJlh/Transformer-Fusion-and-Distillation-model/assets/106720714/ca4c53c0-ea84-4bba-9d03-30aeac06c11d)
## 2. Vision Transformer Fusion
![image](https://github.com/HenryJlh/Transformer-Fusion-and-Distillation-model/assets/106720714/92c574d4-15d1-4b61-8498-e17d6119760f)
## 3. Knowledge Distillation
![image](https://github.com/HenryJlh/Transformer-Fusion-and-Distillation-model/assets/106720714/130f863a-0b80-4e1c-9fcc-0298eac63459)

