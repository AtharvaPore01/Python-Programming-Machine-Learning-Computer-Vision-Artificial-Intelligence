# Lane Line Detector

## Description
Lane Line Detector is a computer vision project that detects and highlights lane lines on road images and videos. The provided code includes two scripts, `lane_detector_image.py` for processing images and `lane_detector_video.py` for processing videos.

## Files

### lane_detector_image.py

- **Author:** Atharva Pore
- **Date:** 25th Dec, 2023

#### Imports
```python
import cv2
import numpy as np
import matplotlib.pyplot as plt
```

#### Functions
- `region_of_interest(image, vertices)`: Defines a mask based on the region of interest.
- `draw_line(image, line_vectors)`: Draws detected lines on a blank image.
- Main code for processing an image, detecting lanes, and displaying the result.

#### Steps to Run 
1. Install Python 3.9.7 and required dependencies:
   - [numpy 1.22.4](https://pypi.org/project/numpy/1.22.4/)
   - [matplotlib 3.4.3](https://pypi.org/project/matplotlib/3.4.3/)
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

3. Update the paths for the image and video in the code.

4. Execute the code through the terminal:
   - **Windows:**
     ```bash
     python lane_detector_image.py
     ```

   - **Mac/Linux:**
     ```bash
     python3 lane_detector_image.py
     ```

### lane_detector_video.py

- **Author:** Atharva Pore
- **Date:** 25th Dec, 2023

#### Imports
```python
import cv2
import numpy as np
import matplotlib.pyplot as plt
```

#### Functions
- `region_of_interest(image, vertices)`: Defines a mask based on the region of interest.
- `draw_line(image, line_vectors)`: Draws detected lines on a blank image.
- `process(image)`: Processes a video frame to detect and draw lane lines.

#### Steps to Run
1. Install Python 3.9.7 and required dependencies (same as for `lane_detector_image.py`).

2. Update the path for the video in the code.

3. Execute the code through the terminal:
   - **Windows:**
     ```bash
     python lane_detector_video.py
     ```

   - **Mac/Linux:**
     ```bash
     python3 lane_detector_video.py  
     ```

## Output Screenshots

### Image Output
![Image Output](https://github.com/AtharvaPore01/Python-Programming-Machine-Learning-Computer-Vision-Artificial-Intelligence/blob/main/RoadLaneLineDetection/output/ImageOutput.png)

### Video Output
![Video Output](https://github.com/AtharvaPore01/Python-Programming-Machine-Learning-Computer-Vision-Artificial-Intelligence/blob/main/RoadLaneLineDetection/output/VideoOutput.png)
```