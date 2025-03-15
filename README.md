
# **SeamCarve: Intelligent Image Resizing**  

![Seam Carving Example](images/example.jpg)  

## **📌 Overview**  
SeamCarve is an advanced **content-aware image resizing** algorithm that intelligently removes or adds seams (low-energy paths) to preserve important details. It utilizes **Numba-optimized dynamic programming** for fast seam removal and real-time visualization.  

## **🚀 Features**  
✔️ **Energy Map Calculation** – Identifies important pixels using gradients  
✔️ **Dynamic Seam Removal** – Finds and removes least important pixels  
✔️ **Parallel Optimization** – Utilizes Numba for performance boost  
✔️ **Vertical & Horizontal Resizing** – Supports both width and height adjustments  
✔️ **Seam Visualization** – Highlights removed seams for better understanding  

## **📦 Installation**  
To set up the project, install the dependencies:  
```bash
pip install numpy opencv-python matplotlib numba
```

## **🛠 Usage**  
Run the script with an image to perform seam carving:  
```bash
python seam_carving.py --image path/to/image.jpg --resize 50
```
Where `--resize 50` reduces the image dimensions by 50%.  

### **🔹 Example Workflow**  
1️⃣ Compute energy map using image gradients  
2️⃣ Detect and remove vertical & horizontal seams  
3️⃣ Display the resized image and visualize removed seams  

## **📸 Example Output**  
| Original Image | Vertical Seam Removal | Horizontal Seam Removal | Resized Image |
|---|---|---|---|
| ![Original](images/original.jpg) | ![Vertical](images/vertical_seams.jpg) | ![Horizontal](images/horizontal_seams.jpg) | ![Resized](images/resized.jpg) |
