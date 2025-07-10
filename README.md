# 🧠 Real-Time Face-Focused Skin Detection using OpenCV

This project is a real-time **skin detection system** using the **YCrCb color space** with OpenCV in Python. It specifically targets **face regions** by applying smart contour filtering based on **area and aspect ratio** to reduce false positives.

https://github.com/user-attachments/assets/0c8b6668-8b03-4b28-a3db-8de78ab3a68a  
<!-- 👉 Tip: If you're uploading the video to GitHub, add it to your repo (e.g., `demo/demo.mp4`) and embed it like this: -->

<!-- ![Demo](demo/demo.gif) or <video src="demo/demo.mp4" controls autoplay loop></video> -->

## 🎯 Features

- ✅ Real-time skin detection via webcam (`cv2.VideoCapture`)
- 🎨 Uses **YCrCb color space**, more robust than RGB for skin tone segmentation
- 🔍 Applies **morphological operations** to clean up the mask
- 🎯 Filters contours by:
  - **Area size** (between 4000 and 50000 pixels)
  - **Aspect ratio** (to approximate face shapes)
- 🖼 Displays both the original frame with detections and the binary mask

## 🚀 Getting Started

### 📦 Requirements

- Python 3.x
- OpenCV
- NumPy

### 🔧 How It Works
1. Converts video frame to YCrCb color space.

2. Applies a skin tone range mask.

3. Cleans the mask using morphological operations (open + close).

4. Finds contours and filters based on:

   - Area to remove small noise or large non-face objects

   - Aspect ratio to ensure the region resembles a face

5. Annotates and draws rectangles around detected skin regions.

# Made with ❤️ using Python & OpenCV.

