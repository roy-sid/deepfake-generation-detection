# Methodology

## 1. Deepfake Generation
- Used DCGAN trained on the CelebA dataset (200K+ faces).
- Generator: 100-D noise vector → 64×64 RGB face image.
- Training stabilized using label smoothing, noise injection, and label flipping.
- Output quality improves over epochs, tracked via saved samples and loss curves.

## 2. Face Swapping (Classical Vision)
- Used MediaPipe FaceMesh (468 landmarks).
- Delaunay triangulation + affine warping + Poisson blending (OpenCV).
- Produced frame-wise swapped face in video using seamlessClone.

## 3. Deepfake Detection
- Dataset: Real-vs-Fake face dataset.
- Model: Pretrained ResNet18, modified for binary classification.
- Accuracy achieved: **96.7%**
- Training loss steadily decreased without overfitting.
