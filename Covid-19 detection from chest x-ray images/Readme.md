# Covid-19 detection from chest X-ray images 

Differentiate between Covid-19, Pneumonia, and the normal case from chest X-ray images

## Dataset description

[COVID19_Pneumonia_Normal_Chest_Xray_PA_Dataset](https://www.kaggle.com/datasets/amanullahasraf/covid19-pneumonia-normal-chest-xray-pa-dataset)

2313 samples for each class (Balanced) - 
6939 samples in total

![covid-dataset-samples](https://github.com/mohdakrory/AI-Based-Medical-Diagnosis-System/assets/67663339/9f8e348d-a40b-457f-b023-77c6b8a7ce41)

## Train test split

**Train:Test -> 0.86:0.13**

**Training set:** 2012 images for each class, with 20% of these images designated for validation, random shuffling was performed per epoch to ensure a diverse and representative training process

**Testing set:** 301 images for each class

 ## Image preprocessing

 All images were normalized and resized to 224*224 with a batch size of 32

## Model architecture

![VGG19+AFR](https://github.com/mohdakrory/AI-Based-Medical-Diagnosis-System/assets/67663339/54d74ec0-8b0c-42d3-a933-e63de63da8be)

## Model performance

**Performance measures on the test set** 

<table>
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
    <td>96.10%</td>
    <td>96.10%</td>
    <td>96.10%</td>
    <td>96.10%</td>
    <td>0.9836</td>
    <td>96.07%</td>
    <td>94.15%</td>
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
    <td>covid</td>
    <td>0.9896</td>
    <td>0.9695</td>
    <td>0.9795</td>
    <td>295</td>
  </tr>
  <tr>
    <td>1</td>
    <td>normal</td>
    <td>0.911</td>
    <td>0.9867</td>
    <td>0.9474</td>
    <td>301</td>
  </tr>
  <tr>
    <td>2</td>
    <td>pneumonia</td>
    <td>0.9894</td>
    <td>0.9269</td>
    <td>0.9571</td>
    <td>301</td>
  </tr>
  <tr>
    <td colspan="2"><b>Accuracy</b></td>
    <td></td>
    <td></td>
    <td>0.961</td>
    <td></td>
  </tr>
  <tr>
    <td colspan="2"><b>Macro Avg</b></td>
    <td>0.9633</td>
    <td>0.961</td>
    <td>0.9613</td>
    <td>897</td>
  </tr>
  <tr>
    <td colspan="2"><b>Weighted Avg</b></td>
    <td>0.9632</td>
    <td>0.961</td>
    <td>0.9612</td>
    <td>897</td>
  </tr>
</table>

**Training and validation curves**

![curves](https://github.com/mohdakrory/AI-Based-Medical-Diagnosis-System/assets/67663339/c1926be0-69b4-40fe-9006-d5e33e764303)

**Confusion matrix visualization**

<table>
  <tr>
    <td>
      <img src="https://github.com/mohdakrory/AI-Based-Medical-Diagnosis-System/assets/67663339/65d0d2d2-1c8d-4dd6-aeae-e1b96122da3a" alt="Image 1">
    </td>
    <td>
      <img src="https://github.com/mohdakrory/AI-Based-Medical-Diagnosis-System/assets/67663339/da7c46d9-3d4f-44aa-9f90-fdc5d6229dc3" alt="Image 2">
    </td>
  </tr>
</table>

## Kaggle notebook for model training

[Notebook](https://www.kaggle.com/code/mohamedeldakrory8/covid-19-chest-x-ray-graduation)
