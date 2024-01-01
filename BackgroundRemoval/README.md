# Background Subtraction Methods in OpenCV

## Description

### createBackgroundSubtractorGMG
The `createBackgroundSubtractorGMG` method in OpenCV performs background subtraction using the GMG (Global Motion-based Background subtraction) algorithm. GMG is based on statistical background modeling and adaptively updates the background.

<details>
<summary>Mathematical Equation</summary>

$`\[ B(x, y, t) = (1 - \alpha) \cdot B(x, y, t-1) + \alpha \cdot I(x, y, t) \]`$
</details>

### createBackgroundSubtractorMOG2
The `createBackgroundSubtractorMOG2` method applies background subtraction using the MOG2 (Mixture of Gaussians) algorithm. MOG2 models each pixel as a mixture of K Gaussian distributions and updates the model over time.

<details>
<summary>Mathematical Equation</summary>

$`\[ P(x, y, t) = \sum_{i=1}^K w_i \cdot \mathcal{N}(x, y, t; \mu_i, \Sigma_i) \]`$
</details>

### createBackgroundSubtractorKNN
The `createBackgroundSubtractorKNN` method performs background subtraction using the KNN (K-nearest neighbors) algorithm. It classifies each pixel as foreground or background based on the K-nearest neighbors in a given neighborhood.

<details>
<summary>Mathematical Equation</summary>

$`\[ P(x, y, t) = \frac{1}{K} \sum_{i=1}^{K} I(x_i, y_i, t) \]`$
</details>

### createBackgroundSubtractorMOG
The `createBackgroundSubtractorMOG` method utilizes the MOG (Mixture of Gaussians) algorithm for background subtraction. Similar to MOG2, it models each pixel as a mixture of K Gaussian distributions but may have differences in the update scheme.

<details>
<summary>Mathematical Equation</summary>

$`\[ P(x, y, t) = \sum_{i=1}^K w_i \cdot \mathcal{N}(x, y, t; \mu_i, \Sigma_i) \]`$
</details>


## Files

### BackgroundRemoval_opencv_python.py
- **Author:** Atharva Pore
- **Date:** 26th Dec, 2023

#### Description
The script demonstrates background subtraction using different methods (GMG, MOG2, KNN, and MOG) in OpenCV. It captures video frames and applies background subtraction, displaying both the original and the foreground mask.

#### Steps to Run
1. Install Python 3.9.7 and required dependencies:
   - [numpy 1.22.4](https://pypi.org/project/numpy/1.22.4/)
   - [opencv-python 4.8.1.78](https://pypi.org/project/opencv-python/4.8.1.78/)

2. Install Anaconda framework on Linux, Mac, and Windows:
   - **Linux:**
     ```bash
     wget https://repo.anaconda.com/archive/Anaconda3-2021.11-Linux-x86_64.sh
     bash Anaconda3-2021.11-Linux-x86_64.sh
     ```

   - **Mac:**
     ```bash
     curl https://repo.anaconda.com/archive/Anaconda3-2021.11-MacOSX-x86_64.pkg -o Anaconda3-2021.11-MacOSX-x86_64.pkg
     sudo installer -pkg Anaconda3-2021.11-MacOSX-x86_64.pkg -target /
     ```

   - **Windows:**
     Download the installer from [Anaconda](https://www.anaconda.com/products/distribution#windows) and follow the installation instructions.

3. Update the path for the video in the code.

4. Execute the code through the terminal:
   - **Windows:**
     ```bash
     python BackgroundRemoval_opencv_python.py
     ```

   - **Mac/Linux:**
     ```bash
     python3 BackgroundRemoval_opencv_python.py
     ```

## Output Screenshots
![Original Image](https://github.com/AtharvaPore01/Python-Programming-Machine-Learning-Computer-Vision-Artificial-Intelligence/blob/main/BackgroundRemoval/output/Original.png)
![Background Removed Image](https://github.com/AtharvaPore01/Python-Programming-Machine-Learning-Computer-Vision-Artificial-Intelligence/blob/main/BackgroundRemoval/output/Background_Removed.png)
