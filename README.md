# Computer-Vision-Project
Setup
1)After downloading the repository, remove all .gitkeep files inside the data folder 
2)KITTI dataset
   Link to Donwload : https://s3.eu-central-1.amazonaws.com/avg-kitti/data_depth_selection.zip 
   Alternatively go to https://www.cvlibs.net/datasets/kitti/eval_depth_all.php and select "Download manually selected validation and test data sets (2 GB)"
Extract val_selection_cropped and insert it into  data/raw folder
3)Nyu Depth v2 dataset
    Go to https://www.kaggle.com/datasets/wesleypan/nyu-depth-v2-labeled-mat and download
    Insert nyu_depth_labeled.mat into data/raw folder
4)Execute prepare_nyu.py and prepare_kitti.py scripts inside the data/scripts folder

