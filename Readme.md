**Kaggle competition**

*Name:* ***SIIM-ACR Pneumothorax Segmentation***

*URL:* ***https://www.kaggle.com/c/siim-acr-pneumothorax-segmentation***

**Download Data into Colab to download dataset**
```
!pip install -q kaggle
from google.colab import files
files.upload()
!mkdir ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
!kaggle competitions download -p "./pneumothorax/" -c siim-acr-pneumothorax-segmentation
!unzip './pneumothorax/stage_2_train.csv.zip' -d './pneumothorax/'
# you have to make account to google cloud and required credientials then download png images, 
# If you don't want to do that download this datasets I found on internet which original dataset. 
!kaggle datasets download -p './data' -d abhishek/siim-png-images
!unzip './data/siim-png-images.zip' -d './data'
# other extra, but same dataset, I found on internet.
# !kaggle datasets download -p "./pneumothorax/other_dataset" -d seesee/siim-train-test
# !unzip './pneumothorax/other_dataset/siim-train-test.zip' -d "./pneumothorax/other_dataset/"
```