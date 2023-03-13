# [Dacon 9th solution] Samsung AI Challenge 3D Metrology

This repository is the ninth-place solution in Samsung AI Challenge (3D-Metrology) organized by Dacon.

The simple data flow chart is specified in the file read.md in Korean. More information can be found in the 삼성 Dacon.pdf file.

Data can be downloaded using the following link.

[Data link](https://dacon.io/competitions/official/235954/data)

The description of the directory and file is as follows.
```bash
├── data
│   ├── simulatin_data
│   │   ├── Depth
│   │   │   ├── Case_1 - 80~84
│   │   │   ├── Case_2 - 80~84
│   │   │   ├── Case_3 - 80~84
│   │   │   └── Case_4 - 80~84
│   │   └── SEM
│   │   │   ├── Case_1 - 80~84
│   │   │   ├── Case_2 - 80~84
│   │   │   ├── Case_3 - 80~84
│   │   │   └── Case_4 - 80~84
│   ├── test
│   │   ├── SEM
│   ├── train
│   │   ├── SEM
│   │   │   ├── Depth_110
│   │   │   ├── Depth_120
│   │   │   ├── Depth_130
│   │   │   └── Depth_140
│   │   └── average_depth.csv
├── submission
├── weight
├── Classification.ipynb
├── Combine-OO.ipynb
├── Image generation.ipynb
├── Segmentation.ipynb
└── 삼성 Dacon.pdf 
```

To obtain the submission.zip file, run the files in the following order:

Firstly, Execute the **`Classfication.ipynb`** file to check that the Depth files in the train folder and the Depth files in simulation_data are paired.

Secondly, Use **`Segmentation.ipynb`** to find the interface that divides the data border and the inside.

More over, **`Image generation.ipynb`** uses simulation data to create new train data by imitating the matched train.

lastly, **`Combine-OO.ipynb`** uses newly created and existing data to estimate the depth map.


![image](https://user-images.githubusercontent.com/79569224/224713116-1f0b86c7-20c0-4fbb-8312-73f631cf7c20.png)

