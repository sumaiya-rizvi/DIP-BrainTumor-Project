



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


![Screenshot 2025-05-19 144144](https://github.com/user-attachments/assets/488fe787-54ed-4cec-8a98-565e445ac712)
![Screenshot 2025-05-19 144242(1)](https://github.com/user-attachments/assets/8c8a52ee-b2bb-48ec-93e3-bf465e7e62f4)
![Screenshot 2025-05-19 144259(1)](https://github.com/user-attachments/assets/e8a46a55-8800-4805-b549-d31ac5cff14d)
![Screenshot 2025-05-19 144327(1)](https://github.com/user-attachments/assets/61c557ad-6f66-43c3-82a5-e7d12592a015)
![Screenshot 2025-05-19 144336(1)](https://github.com/user-attachments/assets/0468e2ed-08f9-442d-b64d-cc60d709e2fa)









