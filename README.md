# video-based-violence-detection
Final project of course "Introduction to Deep learning", CCU, Taiwan
# Code's reference

https://github.com/mchengny/RWF2000-Video-Database-for-Violence-Detection

# Preprocess Data

Remane folder RWF-2000 to RWF

Run notebook: Preprocessing.ipynb

# Re-implement original model: Paper's ACC 84.5, Our's: 84.25

Notebook: Original_Network.ipynb

# Enhance deep feature: Reduce number of conv3d and filter,  add more fully connected layers: ACC 86.25%

Notebook: Enhance_Deep_Feature.ipynb

Best weight (ACC 86.5% on val set): https://drive.google.com/file/d/11UvBe8ZJy09SkKu_d-hhp5XmEPdNMbve/view?usp=sharing

# Enhance deep feature (second): Reduce number of frame per data point, add more fully connected: ACC 86.75%

Notebook: Enhance_Deep_Feature_2.ipynb

Best weight: https://drive.google.com/file/d/1FBPpl-LjLeV72JQznXVeHCbQV7EqOzjD/view?usp=sharing

# Ablation

Goal: Apply other approaches but keep the same number of parameters (or pitiful)

## CNN (as feature extractor - Mobilenet 0.25) + LSTM

Worst, only ACC 60% on val set => no need to store weight

Notebook: CNN_LSTM

## ConvLSTM2D

Notebook: ConvLSTM2D

ACC: 74 val set

Best weight: https://drive.google.com/file/d/1vlA83dcw-gh59SyuqD6_UpmDL0K-FcW_/view?usp=sharing

## Validation

To validation our code, you need to download val.zip and unzip.

Download which ever above model you want.

Using Validation.ipynb notebook.

Change the path to model file (.h5) and val folder.

If you use Colab, you can connect to Google drive and unzip val.zip to drive.

## Demo

Demo Video: https://drive.google.com/file/d/19o42acYtCl6Olo6-mq_nZJ8-Y4tYcxPd/view?usp=sharing

Notebook: Demo.ipynb

Download which ever above model you want.

Download the input video here: https://drive.google.com/file/d/19qW30RlQ2vGWUzoQk621ePYZ_YRrZjMK/view?usp=sharing

Source of video: https://www.youtube.com/watch?v=rDpY91c1ju8

Change the path of model and video input path notebook.





