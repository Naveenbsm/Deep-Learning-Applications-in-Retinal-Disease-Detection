## Deep Learning Applications in Retinal Disease Detection

## Abtract  
Worldwide the  most  common  causes  of  blindness  are  diabetic  retinopathy,  cataract  and glaucoma.  
Timely  detection  is  the  key  to  prevent  blindness  via  retinal  image  screening.  However the  traditional  diagnostics  methods  are  labor  intensive  and  demand  an  expert  to  manage  making it  near  impossible  scale.  
As  the  name  suggests, this  project  focuses  on  deep  learning  solutions  for detecting  retinal  diseases.  More  specifically,  CNN  models  will  be  built  and  contrasted  with Transfer  Learning  using  pre-trained  models  followed  by  a  hybrid  CNN-LSTM  technique.  
The custom CNN performed the best in terms of Accuracy, F1-score &  ROC-AUC, demonstrating its suitability for retinal disease diagnosis. 

## Problem Statement
- Retinal diseases like  diabetic  retinopathy,  cataract  and glaucoma can cause blindness if not detected early

- Manual diagnosis is time consuming and depends on expert availability

- Need for Automated, Scalable AI solutiions

## Objective

- Build deep learning models to classify retinal images
- Compare Performance of:
- Custom CNN
- Transfer learning (VGG16)
- CNN-LSTM

## Dataset
- Source: Kaggle
- Total original images: 3373
- Augmented to: 20,238 images
- Classes:
   - Cataract
   - Diabetic Retinopathy
   - Glaucoma
   - Normal

## Data Preprocessing
- Resized images to 128×128
- Normalization (0–1 range)
- Data augmentation:
   - Rotation
   - Flipping
   - Brightness changes
   - Cropping
 
## Models Used

- ## Custom CNN
- 3 convolution layers + pooling + batch normalization
- Dense layers with dropout
- Best validation accuracy: 85.3%

- ## Transfer Learning (VGG16)
- Pre-trained on ImageNet
- Added custom dense layers
- Frozen base layers initially
- Best validation accuracy: 86.5%

- ## CNN-LSTM
- CNN for spatial features
- LSTM for sequential learning
- Lower performance due to no temporal data

## Results

 | Model      | Accuracy | F1 Score | ROC-AUC |
| ---------- | -------- | -------- | ------- |
| Custom CNN | 86.37%   | 0.8614   | 0.9690  |
| VGG16      | 85.90%   | 0.8590   | 0.9683  |
| CNN-LSTM   | 72.16%   | 0.7070   | 0.9068  |


## Key Findings
- Custom CNN performed best overall
- Transfer learning works well with limited data
- CNN-LSTM underperformed due to lack of temporal features
- Model performance depends heavily on dataset nature

## Tech Stack
- Python
- TensorFlow / Keras
- Scikit-learn
- Matplotlib

## Conclusion
This project demonstrates the effectiveness of deep learning in automated retinal disease detection with CNN based models achieving high diagnostic performance


 
  

