# MM-Point
This is only used to submit code resources related to ACMMM2023 conference papers, to ensure that the double-blind requirements are met

![image](https://github.com/ACMMM-Submission-1018/MM-Point/assets/133339736/200a9a64-168a-4d1a-bcd7-a0ceb6f6be7a)


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

## Dataset preparation

- ModelNet40
- ScanObjectNN
- ShapeNetPart
- S3DIS dataset

Please place the data set file in the 'data' directory of the project system and extract it

---

## Download the pre-trained model weights
> Please note that we upload through Baidu web disk, because the model weight file size is too large. 
**But the Baidu web disk account is a virtual user name, and the author's information has no connection, meet the principle of double blind review.**

### 3D Object Classification——modelNet40
link：https://pan.baidu.com/s/1jEx0KxMggOwktNpHkOWJjA   (code：1018) 

### 3D Object Classification——ScanObjectNN
link：https://pan.baidu.com/s/1O2Qcf04qKKTPmNsnz5RoNA  (code：1018)

Place the downloaded pre-training model file into the "Model" directory of your project system

---

## Downstream Tasks_ 3D Object Classification
Run 'val-modelnet40.ipynb' notebook to perform linear SVM 3D object classification in both **ModelNet40** datasets.

- The classification accuracy of **92.5%** is achieved in the code, **which is higher than reported in the paper**
- as shown in the figure below:
![image](https://github.com/ACMMM-Submission-1018/MM-Point/assets/133339736/552e553c-8c2b-4e7c-a1da-f83e3a4577ed)


Run 'val-scanObjectnn.ipynb' notebook to perform linear SVM 3D object classification in **ScanObjectNN** datasets.
- The classification accuracy of **88.0%** is achieved in the code, **which is higher than reported in the paper**
- as shown in the figure below:
![image](https://github.com/ACMMM-Submission-1018/MM-Point/assets/133339736/f8c82945-73d0-4490-893f-1ab3865cba25)

