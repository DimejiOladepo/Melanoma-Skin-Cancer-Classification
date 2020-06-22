# Melanoma-Skin-Cancer-Classification
<b> <u> Detection of Melanoma Skin Cancer from Dermascopic Images by using Image processing, Noise Reduction techniques and Machine Learning Algorithms to classify Images </u> </b>

Early detection of skin cancer has the potential to reduce mortality and morbidity. Dermoscopy technique is widely used for image acquisition in diagnosis of skin cancer. The aim of this project is to use recently researched de-noising and image processing techniques such as segmentation, image filtering, applying CLAHE to improve images and then transforming these images using their pixel values.

Thereafter, PCA would be applied to reduce image feature size to a size that accounts for 90% of the variance. Classical ML algorithms(K-NN, Logistic Regression and Naive Bayes) willl then be applied to determine the best classifier based on metrics (accuracy, recall, precision, f-1 score, cross-validation score).

The results of this mpdel will be compared to the benchmark model which is the same except the images were not de-noised or further processed. 

<b> The images can be found openly here:</b>

https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/DBW86T

Alternatively, you can download them here:

Link to Original Dermoscopic Image Dataset 
https://drive.google.com/drive/folders/1rUVuoRjL_QgaUi65XlFwy38c43AIMCv_?usp=sharing

Link to feature Engineered Images 
https://drive.google.com/drive/folders/1PlrlGuBbfAFnZGArjY_Mw7WWSCBGrqP0?usp=sharing

#### Libraries Used 
scipy.io
numpy
pandas
matplotlib.pyplot
matplotlib.image
seaborn 
skimage
PIL
skimage
sklearn
fnmatch
os
sys
cv2
warnings

#### Files here include:
- <b> INSTRUCTIONS ON RUNNING THE CLASSIFICATION MODEL.docx </b> - How to run the model
- <b> Skin Cancer Project.pdf </b> - Model Report 
- <b> Skin Submission.ipynb </b> - Model Notebook with code used 
- <b> Skin.html </b> - Model report in html 


###  Result Summary:

<b> Feature Engineered versus Non-Feature Engineered Image set using SVM Classifier </b> 

|  SVM  | Accuracy | Precision | Recall | F1 score | Cross-Validation score |
| --- | --- | --- | --- | --- | --- |
|  Non-FE  | 0.589 | 0.545 | 0.585 | 0.5465 | 0.576
| FE | 0.622 | 0.674 | 0.620 | 0.645 | 0.643 


<b> Feature Engineered SVM versus Feature Engineered Gaussian NB </b>

|  Classifier  | Accuracy | Precision | Recall | F1 score | Cross-Validation score |
| --- | --- | --- | --- | --- | --- |
|  Gaussian NB  | 0.678 | 0.723 | 0.680 | 0.701 | 0.757
| SVM | 0.622 | 0.674 | 0.620 | 0.645 | 0.643 

