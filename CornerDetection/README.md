# Corner Detection With Harris and Shi-Tomasi Methods

## Description

### Harris Corner Detection Method
The Harris Corner Detection code identifies corners in an image based on the variation in intensity in all directions, utilizing the Harris corner detector proposed by Chris Harris and Mike Steffens in 1988. The algorithm involves computing a score "R" for each window, and corners are selected and marked based on a threshold applied to this score.

**Mathematical Equation:**
$`\[ R = \text{det}(\text{M}) - k \cdot (\text{trace}(\text{M}))^2 \]`$

### Shi-Tomasi Corner Detection Method
The Shi-Tomasi Corner Detection code detects corners in an image by utilizing the Shi-Tomasi corner detection method, which is a modification of the Harris corner detector. Corners are identified based on the variation in intensity, and the algorithm selects the most prominent corners in the image.

**Mathematical Equation:**
$`\[ \lambda_{\text{min}} = \min(\lambda_1, \lambda_2) \]`$
$`\[ R = \lambda_{\text{min}} \]`$

## Files

### HarrisCornerDetection.py
- **Author:** Atharva Pore
- **Date:** 27th Dec, 2023

#### Description
The script performs Harris Corner Detection on an image, marking corners based on the computed Harris score. The output image highlights the detected corners in red.

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

3. Update the path for the image in the code.

4. Execute the code through the terminal:
   - **Windows:**
     ```bash
     python HarrisCornerDetection.py
     ```

   - **Mac/Linux:**
     ```bash
     python3 HarrisCornerDetection.py
     ```

### Shi_Tomasi_Method_Corner_Detection.py
- **Author:** Atharva Pore
- **Date:** 27th Dec, 2023

#### Description
The script performs corner detection using the Shi-Tomasi method, marking corners on the image based on the computed eigenvalues. The output image displays the detected corners.

#### Steps to Run
1. Install Python 3.9.7 and required dependencies (same as for `HarrisCornerDetection.py`).

2. Update the path for the image in the code.

3. Execute the code through the terminal:
   - **Windows:**
     ```bash
     python Shi_Tomasi_Method_Corner_Detection.py
     ```

   - **Mac/Linux:**
     ```bash
     python3 Shi_Tomasi_Method_Corner_Detection.py
     ```

## Output Screenshots
![Harris Corner Detection Output](https://github.com/AtharvaPore01/Python-Programming-Machine-Learning-Computer-Vision-Artificial-Intelligence/blob/main/CornerDetection/01-HarrisCornerDetection/output.png)
![Shi-Tomasi Corner Detection Output](https://github.com/AtharvaPore01/Python-Programming-Machine-Learning-Computer-Vision-Artificial-Intelligence/blob/main/CornerDetection/02-Shi_Tomasi_Method/output.png)
