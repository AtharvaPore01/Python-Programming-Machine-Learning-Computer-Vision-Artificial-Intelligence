# Face and Eye Detection

## Description
The Face and Eye Detection code utilizes Haar Cascade classifiers for object detection, proposed by Paul Viola and Michael Jones. It effectively detects faces and eyes in images and videos.

## Files

### FaceEyeDetection_from_Video.py

- **Author:** Atharva Pore
- **Date:** 27th Dec, 2023

#### Description
Haar Cascade Detection is employed for face and eye detection, utilizing pre-trained classifiers. The script processes a video, detects faces, and highlights eyes within those faces.

#### Imports
```python
import cv2
```

#### Steps to Run
1. Install Python 3.9.7 and required dependencies:
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

3. Update the paths for the video and classifiers in the code.

4. Execute the code through the terminal:
   - **Windows:**
     ```bash
     python FaceEyeDetection_from_Video.py
     ```

   - **Mac/Linux:**
     ```bash
     python3 FaceEyeDetection_from_Video.py
     ```

### FaceEyeDetection_from_Image.py

- **Author:** Atharva Pore
- **Date:** 27th Dec, 2023

#### Description
Haar Cascade Detection is employed for face and eye detection, utilizing pre-trained classifiers. The script processes an image, detects faces, and highlights eyes within those faces.

#### Imports
```python
import cv2
```

#### Steps to Run
1. Install Python 3.9.7 and required dependencies (same as for `FaceEyeDetection_from_Video.py`).

2. Update the paths for the image and classifiers in the code.

3. Execute the code through the terminal:
   - **Windows:**
     ```bash
     python FaceEyeDetection_from_Image.py
     ```

   - **Mac/Linux:**
     ```bash
     python3 FaceEyeDetection_from_Image.py
     ```

## Output Screenshots
(https://github.com/AtharvaPore01/Python-Programming-Machine-Learning-Computer-Vision-Artificial-Intelligence/blob/main/FaceEyeDetection/output/output.png)
```