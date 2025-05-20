



#  Brain Tumor MRI Image Filtering and Denoising using Classical DIP Techniques

This project focuses on **enhancing and preprocessing brain MRI images** by applying **Digital Image Processing (DIP)** techniques. The goal is to **remove noise**, highlight important structures, and segment potential tumor regions using **classical methods**, without deep learning.

It also includes a **Streamlit web app** for user-friendly interaction with the filtering and segmentation pipeline.



## Project Objectives

* Apply **classical image filtering** techniques to remove noise from brain MRI scans.
* Use **thresholding, morphological operations**, and **contour detection** to segment possible tumor regions.
* Provide an **interactive interface** for uploading and processing MRI images via **Streamlit**.


##  Techniques Implemented

###  Image Filtering Techniques:

* **Gaussian Filtering** – smoothens image and reduces Gaussian noise.
* **Median Filtering** – removes salt-and-pepper noise while preserving edges.
* **Bilateral Filtering** – reduces noise while keeping edges sharp.

###  Segmentation & Enhancement Techniques:

* **Otsu’s Thresholding** – automatic threshold value to binarize the image.
* **Morphological Operations** – dilation, erosion, opening, and closing to refine binary masks.
* **Contour Detection** – extract object boundaries to highlight tumor region.

###  Feature Extraction:

* **Area**
* **Perimeter**
* **Bounding box**
* **Centroid (optional)**



## 🗂️ Project Structure

```bash
BrainTumorMRI-Denoising-DIP/
│
├── brain_tumor_app.py             # Streamlit App file
├── filtering.py                   # Filtering methods (Gaussian, Median, Bilateral)
├── segmentation.py                # Thresholding and morphological operations
├── utils.py                       # Helper functions (loading, feature extraction)
├── images/                        # Folder containing input MRI images
├── output/                        # Processed and segmented images (masks, overlays)
├── requirements.txt               # Python dependencies
└── README.md                      # Project documentation
```



##  How to Run the Project

>  Make sure Python and required packages are installed on your system.

###  Step 1: Clone the Repository

```bash
git clone https://github.com/sumaiya-rizvi/BrainTumorMRI-Denoising-DIP.git
cd BrainTumorMRI-Denoising-DIP
```

###  Step 2: Install Required Libraries

You can use `pip`:

```bash
pip install -r requirements.txt
```

Or install them manually:

```bash
pip install streamlit opencv-python numpy matplotlib
```

### 🧠 Step 3: Run the Streamlit App

```bash
streamlit run brain_tumor_app.py
```

The app will open in your default browser. You can upload an MRI image, apply filters, segment the tumor, and view results.


##  Features of the App

*  Upload MRI brain scan images
*  Choose and apply different filters:

  * Gaussian
  * Median
  * Bilateral
*  Apply Otsu’s Thresholding and Morphological Operations
*  View segmented tumor region
*  View extracted features: **Area**, **Perimeter**, etc.
*  Save processed output images



## 🖼 Sample Results

| Original Image          | Filtered Image            | Thresholded + Segmented    |
| ----------------------- | ------------------------- | -------------------------- |
| ![](images/sample1.png) | ![](output/filtered1.png) | ![](output/segmented1.png) |



##  Author

**Sumaiya Rizvi**
BS Artificial Intelligence
Digital Image Processing Final Project



##  License

This project is for educational purposes and may be used under the [MIT License](LICENSE).


### DEMO (OUTPUT)

![Screenshot 2025-05-19 144144(1)](https://github.com/user-attachments/assets/3a498637-d4e5-4770-b11c-86a693f60a25)
![Screenshot 2025-05-19 144203(1)](https://github.com/user-attachments/assets/74f568e8-89ae-4c97-ade1-d7f3ebb456e8)
![Screenshot 2025-05-19 144242(1)](https://github.com/user-attachments/assets/83bbd383-fb61-4a21-bbf6-78a5b7cc1194)
![Screenshot 2025-05-19 144259(1)](https://github.com/user-attachments/assets/eb02f896-783d-4760-8ae3-1820d6e046b7)
![Screenshot 2025-05-19 144317(1)](https://github.com/user-attachments/assets/e0ddc9fe-85f7-46d8-8013-21fafafe2dee)
![Screenshot 2025-05-19 144327(1)](https://github.com/user-attachments/assets/f7138cd2-8f5c-458e-9f2c-1fccfce9b6b3)
![Screenshot 2025-05-19 144336(1)](https://github.com/user-attachments/assets/9712822f-c189-45f6-ba48-8334779edfa7)















