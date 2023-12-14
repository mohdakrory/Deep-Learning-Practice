Covid-19 detection from chest X-ray images 
--

Differentiate between Covid-19, Pneumonia, and the normal case from chest X-ray images

**Dataset description**

[COVID19_Pneumonia_Normal_Chest_Xray_PA_Dataset](https://www.kaggle.com/datasets/amanullahasraf/covid19-pneumonia-normal-chest-xray-pa-dataset)

2313 samples for each class (Balanced) - 
6939 samples in total

![covid-dataset-samples](https://github.com/mohdakrory/AI-Based-Medical-Diagnosis-System/assets/67663339/9f8e348d-a40b-457f-b023-77c6b8a7ce41)

**Proposed model**

![VGG19+AFR](https://github.com/mohdakrory/AI-Based-Medical-Diagnosis-System/assets/67663339/54d74ec0-8b0c-42d3-a933-e63de63da8be)

**Model performance**

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

![curves](https://github.com/mohdakrory/AI-Based-Medical-Diagnosis-System/assets/67663339/c1926be0-69b4-40fe-9006-d5e33e764303)

![image](https://github.com/mohdakrory/AI-Based-Medical-Diagnosis-System/assets/67663339/0b0674c2-d7dd-44a7-9dd6-660f23a696ac)

**Kaggle notebook for model training**

[Notebook](https://www.kaggle.com/code/mohamedeldakrory8/covid-19-chest-x-ray-graduation)
