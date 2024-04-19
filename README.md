# Transformer-Fusion-and-Distillation-model
## Abstract
This paper shows the potential of ViT model (Vision Transformer) to achieve multi-modal fusion based on a case implementation of "cortical cataract intelligent grading". This project intends to learn pathological features that are in line with clinical judgment by multi-modal fusion of image and sub-label from local features. At the same time, a distillation network framework is proposed to eliminate the input of sub-label in the test, so that better classification results can be obtained by relying on images alone. 
## Methods
Our framework design is mainly divided into three parts: Firstly, image features and text features (sub-label features) are extracted based on residual network and deep neural network, respectively. Secondly, the multi-modal fusion of image and text features is realized by using ViT model framework. Finally, the trained high-precision fusion model is used to guide the learning of residual network through knowledge distillation to achieve no sublabel input and improve the accuracy of image unimodal. Our high-precision fusion model achieves 93.02% accuracy on the cortical cataract dataset, and the residual network of knowledge distillation achieves 79.27% accuracy without sublabel input, which is nearly 5% higher than that of residual network alone.
## 1. Features Extraction
![image](https://github.com/HenryJlh/Transformer-Fusion-and-Distillation-model/assets/106720714/91a8dec4-ebcb-45a0-ac95-24e02c1d8db2)
## 2. Vision Transformer Fusion
![image](https://github.com/HenryJlh/Transformer-Fusion-and-Distillation-model/assets/106720714/fe311341-5e0b-4a8e-9c75-cd2ef31e19d3)
## 3. Knowledge Distillation
![image](https://github.com/HenryJlh/Transformer-Fusion-and-Distillation-model/assets/106720714/24a1b6f2-899e-4e81-aff1-15de64dcf4e4)

