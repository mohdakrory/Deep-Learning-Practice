# Brain tumor detection from MRI images  

Differentiate between Meningioma, Glioma, Pituitary, and the normal case from MRI images 

## Dataset description

[Brain Tumor MRI Dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)

**Dataset samples**

![brain-tumor-dataset-samples](https://github.com/mohdakrory/AI-Based-Medical-Diagnosis-System/assets/67663339/6664e7c6-54e4-4ffd-866d-c4ae71d358b3)

**Class distribution and train-test split**

![image](https://github.com/mohdakrory/AI-Based-Medical-Diagnosis-System/assets/67663339/4ab77fde-e07c-41d7-8009-cdb8613b9f55)
![image](https://github.com/mohdakrory/AI-Based-Medical-Diagnosis-System/assets/67663339/10551bbf-85cb-4bff-b4ca-8d2810fdc124)

 ## Image preprocessing

 All images were normalized, converted to gray scale,and resized to 64*64 with a batch size of 32
 
## Model architecture

![brain tumor framework](https://github.com/mohdakrory/Deep-Learning-Practice/assets/67663339/76b87e4b-7def-4106-95a8-e48096e707f1)

## Model performance

**Performance measures on the test set** 

<table border="1">
  <tr>
    <th>Accuracy</th>
    <th>Precision</th>
    <th>Recall</th>
    <th>F1</th>
    <th>AUC</th>
    <th>G-mean</th>
    <th>Kappa</th>
  </tr>
  <tr>
    <td>99.08%</td>
    <td>99.08%</td>
    <td>99.01%</td>
    <td>99.04%</td>
    <td>0.9998</td>
    <td>98.34%</td>
    <td>97.67%</td>
  </tr>
</table>

**Classification report**

<table border="1">
  <tr>
    <th>Index</th>
    <th>Class Name</th>
    <th>Precision</th>
    <th>Recall</th>
    <th>F1-Score</th>
    <th>Support</th>
  </tr>
  <tr>
    <td>0</td>
    <td>glioma</td>
    <td>0.9966</td>
    <td>0.9833</td>
    <td>0.9899</td>
    <td>300</td>
  </tr>
  <tr>
    <td>1</td>
    <td>meningioma</td>
    <td>0.9804</td>
    <td>0.9804</td>
    <td>0.9804</td>
    <td>306</td>
  </tr>
  <tr>
    <td>2</td>
    <td>notumor</td>
    <td>0.9926</td>
    <td>1</td>
    <td>0.9963</td>
    <td>405</td>
  </tr>
  <tr>
    <td>3</td>
    <td>pituitary</td>
    <td>0.9934</td>
    <td>0.9967</td>
    <td>0.995</td>
    <td>300</td>
  </tr>
  <tr>
    <td colspan="6"></td>
  </tr>
  <tr>
    <td>Accuracy</td>
    <td colspan="3"></td>
    <td>0.9908</td>
    <td>897</td>
  </tr>
  <tr>
    <td>Macro Avg</td>
    <td></td>
    <td>0.9908</td>
    <td>0.9901</td>
    <td>0.9904</td>
    <td>897</td>
  </tr>
  <tr>
    <td>Weighted Avg</td>
    <td></td>
    <td>0.9909</td>
    <td>0.9908</td>
    <td>0.9908</td>
    <td>897</td>
  </tr>
</table>


**Training and validation curves**

![curves](https://github.com/mohdakrory/AI-Based-Medical-Diagnosis-System/assets/67663339/bae028d9-92a7-4d5e-9dfc-00c003a749fc)

**Confusion matrix visualization**

<table>
  <tr>
    <td>
      <img src="https://github.com/mohdakrory/AI-Based-Medical-Diagnosis-System/assets/67663339/f8f5e671-3c58-4962-906d-edfe7147c31e">
    </td>
    <td>
      <img src="https://github.com/mohdakrory/AI-Based-Medical-Diagnosis-System/assets/67663339/05d37008-566c-4c18-bf95-bf47b2912f3d">
    </td>
  </tr>
</table>

## Kaggle notebook for model training

[Notebook](https://www.kaggle.com/code/mohamedeldakrory8/brain-tumor-mri-classification-graduation)

