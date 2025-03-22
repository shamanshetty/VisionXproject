# Reflection Removal Model 🪞➡️🖼  

## Overview  
This project implements a **deep learning model** for **reflection removal from images**. Developed during **VisionX Hackathon (Qualcomm)**, our model enhances image quality by eliminating unwanted reflections using a **Convolutional Neural Network (CNN)**.  

## Features  
✔ **Removes reflections** from glass-covered images.  
✔ **Deep learning-based** approach using **TensorFlow/Keras**.  
✔ **Custom dataset handling** for training and evaluation.  
✔ **Automated preprocessing** with image augmentation.  
✔ **Model checkpointing** for optimized training.  
✔ **Evaluation & visualization** of results.  

## Technologies Used  
- **Python**  
- **TensorFlow / Keras**  
- **OpenCV**  
- **NumPy & Matplotlib**  
- **PIL (Pillow)**  

## Dataset  
The dataset consists of:  
📂 **With Reflection** – Images containing reflections.  
📂 **Without Reflection** – Ground truth images (reflection-free).  
📂 **Test Cases** – Unseen images for evaluation.  

## Installation & Setup  
### Prerequisites  
Ensure you have Python **3.7+** installed along with the required dependencies.  

### Install Dependencies  
```bash
pip install -r requirements.txt
```  

### Running the Model  
1. **Prepare your dataset**: Ensure you have folders for images with and without reflections.  
2. **Train the model**:  
   ```bash
   python train.py
   ```  
3. **Test the model** on new images:  
   ```bash
   python test.py --input test_images --output results/
   ```  
4. **Visualize results**: The script generates side-by-side comparisons of input vs. output.  

## Model Architecture  
The model follows a **U-Net inspired CNN architecture**, consisting of:  
- **Convolutional layers** for feature extraction.  
- **Downsampling & Upsampling** to reconstruct reflection-free images.  
- **Skip connections** to retain important features.  
- **Activation: ReLU & Sigmoid** for precise pixel-wise predictions.  

## Evaluation Metrics  
📊 The model is evaluated using:  
- **PSNR (Peak Signal-to-Noise Ratio)**  
- **SSIM (Structural Similarity Index)**  
- **MSE (Mean Squared Error)**  

## Contributions  
🚀 Contributions are welcome! If you have suggestions, improvements, or bug fixes, feel free to:  
1. **Fork the repository**  
2. **Create a new branch**  
3. **Submit a Pull Request**  

---

🔬 **Developed for VisionX Hackathon by Qualcomm**  
💡 **Team Name:** *WESHOWSPEED*  

🚀 **Removing Reflections, Enhancing Reality!**
