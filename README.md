# Brain-tumor-detection-using-CNNs-and-transfer-learning-on-MRI-scans
## Project Overview
A comprehensive comparative analysis on CNN models - LeNet, AlexNet, ZFNet,  VGGNet, GoogLeNet, and ResNet50 on a dataset comprising 10287 MRI images across four  classes: glioma, meningioma, pituitary tumors, and non-tumor cases also investigated the efficacy of transfer learning using a pre trained VGG16 model with ImageNet weights
# Brain Tumor Detection Using CNNs & Transfer Learning on MRI Scans

---

## Dataset
- **Total images:** 10,287  
- **Classes:** Glioma, Meningioma, Pituitary Tumor, Non-Tumor  
- **Image preprocessing:** resizing, normalization  
- **Note:** Dataset folder path must be updated inside the notebooks.

---

## Models Implemented
The following models are implemented across the two notebooks:

### From `CNN models.ipynb`:
- LeNet  
- AlexNet  
- VGGNet  
- GoogLeNet (Inception)  
- ResNet50  
- VGG16 (Transfer Learning)

### From `zfnet.ipynb`:
- ZFNet (custom implementation with convolutional + pooling blocks)

---

## Methodology
1. Load MRI images from directories  
2. Preprocess images (resize → normalize)  
3. Encode class labels  
4. Train/validation split (user can modify in notebook)  
5. Train each CNN architecture  
6. Track:
   - Training/validation accuracy  
   - Training/validation loss  
7. Evaluate each model  
8. Predict sample MRI images (via `predict_image()` in ZFNet notebook)

---

## Results
Actual accuracy values are not printed in the uploaded notebooks.  
Below is the table template for updating results after running the models:

| Model        | Test Accuracy | Notes |
|--------------|--------------:|-------|
| LeNet        |    91.79%     | Baseline CNN |
| AlexNet      |    92.55%     | Classic deep CNN |
| ZFNet        |    93.72%     | Implemented in `zfnet.ipynb` |
| VGGNet       |    93.72%     | Deep architecture |
| GoogLeNet    |    66.57%     | Inception modules |
| ResNet50     |    92.08%     | Residual learning |
| VGG16 (TL)   |    93.02%     | Transfer learning using ImageNet |

---

## Project Applications
- MRI-based tumor detection  
- Radiology decision-support  
- Automated medical image classification  

