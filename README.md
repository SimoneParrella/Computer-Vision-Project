# Computer-Vision-Project
Setup
-After downloading the repository, remove all .gitkeep files inside the data folder 
-KITTI dataset
1) Link to Donwload : https://s3.eu-central-1.amazonaws.com/avg-kitti/data_depth_selection.zip 
   Alternatively go to https://www.cvlibs.net/datasets/kitti/eval_depth_all.php and select "Download manually selected validation and test data sets (2 GB)"
2)Extract val_selection_cropped and insert it into  data/raw folder
-Nyu Depth v2 dataset
 1) Go to https://www.kaggle.com/datasets/wesleypan/nyu-depth-v2-labeled-mat and download
 2) Insert nyu_depth_labeled.mat into data/raw folder
-Execute prepare_nyu.py and prepare_kitti.py
