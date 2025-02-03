# Trash classification using SVM

## About
This repository contains the final project that consists code and paper of me and my team (Jiin Park, Hawk He, Rinnie Chen, and Jayden Gordon) during 31256 Image Processing and Pattern Recognition at UTS. The model is fully written in Python and trained using Google Colab. Our project used TensorFlow, Sci-kit, and MobileNetV2 for data preparation and training.

## Dataset & Training
We used data from [TrashNet](https://www.kaggle.com/datasets/feyzazkefe/trashnet/data) to train our model. The model used an 80/20 split for training/validation. In this paper, we tried 2 models to train the data, CNN and SVM.


## Results

#### CNN

| Type | Precision     | recall                     | f1-score   |   support    |
| :-------- | :------- | :------------------------- | :------|:------|
| `cardboard` | 0.11 |0.07 |     0.09   |  80   |
| `glass` | 0.23 |    0.35    |    0.28    |  100    |
| `metal` | 0.17` | 0.18|       0.18 |   82   |
| `paper` | 0.30 |  0.35|     0.32   |   118   |
| `plastic` | 0.26 |  0.11|      0.16  |   96    |
| `trash` | 0.04 |  0.04|       0.04 |   27    |

Average accuracy: 22%
#### SVM (Reinforced with MobileNetV2)

| Type | Precision     | recall                     | f1-score   |   support    |
| :-------- | :------- | :------------------------- | :------|:------|
| `cardboard` | 0.93 |0.66 |  0.77      |  80     |
| `glass` | 0.64 |   0.79     |   0.28     | 100      |
| `metal` | 0.76 | 0.83|    0.80    |  82     |
| `paper` | 0.71 | 0.93 |   0.81     |   118    |
| `plastic` | 0.71 | 0.51 |     0.59   | 0.96      |
| `trash` | 0.64 | 0.26 |  0.37      |   27    |

Average accuracy: 73%



## Acknowledgements

 - [Gary Thung and Mindi Yang's Trashnet Github](https://github.com/garythung/trashnet)


