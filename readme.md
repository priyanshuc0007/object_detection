# 🖼️ **Object Detection with OpenCV and DETR**

This Python script uses **OpenCV** and the **DETR (DEtection TRansformer)** model for real-time object detection via webcam.

---

## 🔧 **Libraries Used**
- **cv2**: OpenCV for computer vision tasks.
- **transformers**: Hugging Face library for object detection.
- **torch**: PyTorch deep learning framework.
- **PIL**: Image processing with Python Imaging Library.

---

## 🚀 **Initialization**
- **DETR Model & Processor**: Initialized from Hugging Face's Transformers.
- **Webcam Capture**: Set up using OpenCV's `VideoCapture`.

---

## 🔄 **Main Loop Overview**
1. **Capture Frame**: Continuously captures frames via webcam.
2. **Convert Frame**: Converts from BGR to RGB format.
3. **Process Frame**: Prepares the frame for detection with PIL and the image processor.
4. **Object Detection**: DETR model detects objects.
5. **Post-Processing**: Extracts bounding boxes, labels, and confidence scores.
6. **Draw Bounding Boxes**: Overlays bounding boxes and labels on detected objects.
7. **Display Frame**: Displays the frame with detections using `imshow`.
8. **Exit Condition**: Press 'q' to exit the loop.

---

## 🧹 **Cleanup**
- Releases webcam: `cap.release()`.
- Closes OpenCV windows: `cv2.destroyAllWindows()`.

---

## 📋 **Usage**
1. Install necessary libraries: `cv2`, `transformers`, `torch`, and `PIL`.
2. Run the script to start the webcam feed with real-time object detection.
3. Press 'q' to quit.

---

## 📦 **Dependencies**
- **OpenCV**
- **Hugging Face Transformers**
- **PyTorch**
- **PIL**
