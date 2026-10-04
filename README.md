# Computer-Vision-Project

Out-of-distribution (OOD) detection for Monocular Depth Estimation. This project adapts **CORES** (COnvolutional REsponse-based Score) — originally designed for classification — to two dense-prediction architectures, **FastDepth** and **METER**, trained on **NYU Depth V2** (in-distribution) and evaluated against **KITTI** (out-of-distribution). The goal is to test whether a network's internal convolutional responses alone can separate ID and OOD inputs, without relying on class logits.

## Setup

### 1. Clone the repository

After downloading the repository, remove all `.gitkeep` files inside the `data` folder.

### 2. Download the datasets

**KITTI** (OOD evaluation)

- Download: [data_depth_selection.zip](https://s3.eu-central-1.amazonaws.com/avg-kitti/data_depth_selection.zip)
- Alternatively, go to the [KITTI depth evaluation page](https://www.cvlibs.net/datasets/kitti/eval_depth_all.php) and select "Download manually selected validation and test data sets (2 GB)"
- Extract `val_selection_cropped` into `data/raw`

**NYU Depth V2** (training / ID)

- Download from [Kaggle: nyu-depth-v2-labeled-mat](https://www.kaggle.com/datasets/wesleypan/nyu-depth-v2-labeled-mat)
- Place `nyu_depth_labeled.mat` into `data/raw`

### 3. Prepare the data

Run the preprocessing scripts in `data/scripts`:

```bash
python data/scripts/prepare_nyu.py
python data/scripts/prepare_kitti.py
```
