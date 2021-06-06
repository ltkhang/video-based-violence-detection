# video-based-violence-detection
Final project of course "Introduction to Deep learning", CCU, Taiwan
# Code's reference

https://github.com/mchengny/RWF2000-Video-Database-for-Violence-Detection

# Preporcess Data

Remane folder RWF-2000 to RWF

Run notebook: Preprocessing.ipynb

# Re-implement original model

Notebook: Original_Network.ipynb

# Enhance deep feature (more Fully connected layer)

Notebook: Enhance_Deep_Feature.ipynb

Best weight (ACC 86.5% on val set): https://drive.google.com/file/d/11UvBe8ZJy09SkKu_d-hhp5XmEPdNMbve/view?usp=sharing

# Ablation

Goal: Apply other approaches but keep the same number of parameters (or pitiful)

## CNN (as feature extractor - Mobilenet 0.25) + LSTM

Worst, only ACC 60% on val set => no need to store weight

Notebook: CNN_LSTM

## ConvLSTM2D

Notebook: ConvLSTM2D

ACC: 74 val set

Best weight: https://drive.google.com/file/d/1vlA83dcw-gh59SyuqD6_UpmDL0K-FcW_/view?usp=sharing



