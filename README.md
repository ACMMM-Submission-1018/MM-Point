# MM-Point
This is only used to submit code resources related to the ACMMM2023 conference papers.

Currently, the submitted project code resources contain the verification part of the experimental results for the supplementary material part of the paper submission. 

At the same time, no information related to the author can be disclosed, and this GitHub account is a new account created temporarily for the purpose of this submission, to ensure that the double-blind requirements are met.

- Anonymous Author(s)
- Submission Id: 1018


![image](https://github.com/ACMMM-Submission-1018/MM-Point/assets/133339736/abc05618-91d2-4fb0-8e5e-f39138f52e10)


![image](https://github.com/ACMMM-Submission-1018/MM-Point/assets/133339736/200a9a64-168a-4d1a-bcd7-a0ceb6f6be7a)

---
---

## Unique project code address on GitHub 
- currently only used for supporting material in paper review: https://github.com/ACMMM-Submission-1018/MM-Point/

---
---

## The setting of the code runtime environment
- pytorch> 1.9.0
- torchvision
- pillow
- numpy
- h5py
- lightly
- scikit-learn
- h5py

---
---

## Dataset preparation

- ModelNet40
- ScanObjectNN
- ShapeNetPart
- S3DIS dataset

Please place the data set file in the 'data' directory of the project system and extract it

---
---

## Download the pre-trained model weights
> Please note that we upload through Baidu web disk, because the model weight file size is too large. 
**But the Baidu web disk account is a virtual user name, and the author's information has no connection, meet the principle of double blind review.**

### 3D Object Classification——modelNet40
link：https://pan.baidu.com/s/1jEx0KxMggOwktNpHkOWJjA  (code：1018) 

### 3D Object Classification——ScanObjectNN
link：https://pan.baidu.com/s/1O2Qcf04qKKTPmNsnz5RoNA  (code：1018)

### 3D Object Classification——modelNet10
link：https://pan.baidu.com/s/1l3I4vaY-LSADIwszxAHTCw  (code：1018)

Place the downloaded pre-training model file into the "Model" directory of your project system

---
---

## Downstream Tasks_ 3D Object Classification
1. Run 'val-modelnet40.ipynb' notebook to perform linear SVM 3D object classification in both **ModelNet40** datasets.

- The classification accuracy of **92.5%** is achieved in the code, **which is higher than reported in the paper**
- as shown in the figure below:
![image](https://github.com/ACMMM-Submission-1018/MM-Point/assets/133339736/552e553c-8c2b-4e7c-a1da-f83e3a4577ed)

---

2. Run 'val-scanObjectnn.ipynb' notebook to perform linear SVM 3D object classification in **ScanObjectNN** datasets.
- The classification accuracy of **88.0%** is achieved in the code, **which is higher than reported in the paper**
- as shown in the figure below:
![image](https://github.com/ACMMM-Submission-1018/MM-Point/assets/133339736/f8c82945-73d0-4490-893f-1ab3865cba25)

---

3. Run 'val-modelnet10.ipynb' notebook to perform linear SVM 3D object classification in **ModelNet10** datasets.
- The classification accuracy of **95.4%** is achieved in the code. This is the same as reported in the paper.
- as shown in the figure below:
![image](https://github.com/ACMMM-Submission-1018/MM-Point/assets/133339736/19773ea2-81ac-4f3b-b048-f856cb6370df)

### Please note 
- We are using **two 3090GPUs of 24G size in our experiment**. 
- Please modify the batch-size, num-workers, and other parameters according to your actual hardware environment
