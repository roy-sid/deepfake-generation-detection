# 🧠 Deepfake Generation and Detection

This project is an end-to-end deep learning pipeline that performs both **deepfake generation** using GANs and **deepfake detection** using a CNN classifier. Built with PyTorch and trained on publicly available Kaggle datasets.

---

## 📂 Project Highlights

### 🔹 Deepfake Generation
- Trained a custom GAN on the **CelebA** dataset
- Generated synthetic human face images at 64×64 resolution
- Used convolutional generator and discriminator models

### 🔹 Deepfake Detection
- Used a CNN-based classifier (e.g. ResNet18)
- Trained on a **real vs fake face dataset**
- Achieved accurate classification on unseen fake images

---

## 📦 Datasets Used

1. **[CelebA Face Dataset](https://www.kaggle.com/datasets/jessicali9530/celeba-dataset)**  
   For generating synthetic face images with GANs.

2. **[Real and Fake Face Detection Dataset](https://www.kaggle.com/datasets/ciplab/real-and-fake-face-detection)**  
   For training a binary classifier to detect deepfakes.

---

## 🛠️ Tech Stack

- Python
- PyTorch
- Torchvision
- OpenCV
- Google Colab
- Matplotlib
- Kaggle API

---

## 🚀 Running the Project

1. Upload your `kaggle.json` file and authenticate Kaggle API
2. Download the datasets using:
   ```bash
   !kaggle datasets download -d jessicali9530/celeba-dataset
   !kaggle datasets download -d ciplab/real-and-fake-face-detection

3. Run the notebook `deepfake_pipeline.ipynb` step-by-step

4. Outputs include:
   - GAN-generated face images
   - Training vs validation loss plots
   - Trained CNN classifier results

---

## 📊 Outputs

- ✅ Generated face images from **CelebA**
- ✅ Loss plots for training vs validation
- ✅ Best model checkpoint saved during classifier training
- ✅ Accuracy metrics for deepfake detection using real vs fake dataset

---

## 🙋‍♂️ Author

**Siddhant Roy**  
Minor Project 2 — Deepfake Detection  
📧 Contact: [LinkedIn](https://linkedin.com/) | [GitHub](https://github.com/)

