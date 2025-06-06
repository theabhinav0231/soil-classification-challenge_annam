# Annam.ai Soil Classification Hackathon

The repository has 2 directories for 2 challenges that were provided in Annam.ai Hackathon.

The files for submission are also listed here-


Video URL- https://drive.google.com/drive/folders/1UdhJYSvxAE5-2d6GEqAF1aOeOX8JLqBI?usp=sharing


Transcript File- https://drive.google.com/file/d/1xl5z2g3-Hq4MaclJxRzDlvpS-7XrzplZ/view?usp=sharing

## 🛠️ Getting Started

1. **Clone the repo**  
   ```bash
   git clone https://github.com/theabhinav0231/soil-classification-challenge_annam.git
   cd soil-classification-challenge_annam

2. **Install dependencies (optional if using Google Colab):**
  ```bach
  pip install -r requirements.txt
   ```

## 📥 Dataset Download (from Kaggle)

This project uses a dataset from a Kaggle competition: **Soil Classification 2025**.  
To download the dataset automatically, use the provided `download.sh` script for both the challenge directories.

---

### 🧩 Setup Instructions

To get started:

#### 1. Install Kaggle CLI  
```bash
pip install kaggle
```

### Set up your Kaggle API credentials

To access the dataset from Kaggle via script:

1. Go to your [Kaggle Account Settings](https://www.kaggle.com/account)
2. Click **"Create New API Token"**
3. This will download a file named `kaggle.json`

Now move the file to the appropriate location on your system:

```bash
mkdir -p ~/.kaggle
mv /path/to/kaggle.json ~/.kaggle/
chmod 600 ~/.kaggle/kaggle.json
```

### Run the Dataset Download Script

Once your Kaggle API credentials are set up, run the script provided in the root of this repository:

```bash
chmod +x download.sh
./download.sh
```

After running, your dataset will be available under:
data/soil_classification-2025/



### **Important Note For Running Inference notebooks**
Challenge-1: After running the training.ipynb file, there will be 5 models saved in your output directory. Please download those model.pth files locally and and make sure to upload it in input directory before running inference.ipynb.


Challenge-2: After running the training_.ipynb file, there will be 5 models saved in your output directory. Based on the F1 score, please download the best performing model.pth file and upload it in the input directory before running inference_.ipynb file.


Launch Jupyter Notebook or use Google Colab to open the .ipynb files.


**License**

**This repository is released under the MIT License.**
