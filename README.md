# Brain Tumor Detection Using CNN

## Project Overview
This project aims to detect the presence of brain tumors in MRI images using Convolutional Neural Networks (CNNs) and transfer learning. The dataset consists of a small number of labeled MRI scans (~253 images), divided into two classes:  
- **0**: No tumor  
- **1**: Tumor  

Due to the small dataset size, training deep learning models presents unique challenges.

---

## Dataset
- The dataset contains MRI images labeled as “tumor” or “no tumor.”  
- Class distribution is imbalanced, with the majority being tumor images.  
- Images were preprocessed and resized to 224x224 pixels.   

---

## Models Implemented
1. **CNN**  
   - Achieved ~57–69% accuracy on the test set.  
   - Confusion matrix indicates the model tends to predict the majority class.  

2. **Transfer learning (MobileNetV2)**  
   - Performance was worse than CNN (~42% accuracy).  
   - Likely due to insufficient data for fine-tuning pretrained networks.  

---

## Key Findings
- **CNN** performed better than transfer learning on this small dataset.  
- **Class imbalance** caused poor predictions for the “no tumor” class.  
- **Data augmentation** helped slightly but did not increase the actual dataset size, limiting improvements.  

---

## Limitations
- **Tiny dataset** limits model performance and generalization.  
- **Class imbalance** reduces accuracy for minority class predictions.  
- **Transfer learning is less effective** on very small medical image datasets.  

---

## Recommendations
- Collect more labeled MRI images to increase dataset size.    
- For very small datasets, simpler CNN architectures or classical ML methods with feature extraction may perform better.   

---

