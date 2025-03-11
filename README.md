# AI-Powered Security Camera with YOLO-NAS

## 1. Introduction
This project implements an AI-powered security camera system using **YOLO-NAS** for real-time object detection. The system is capable of detecting accidents and suspicious activities in both images and videos. It integrates **Google Firebase** for secure access control and employs **Streamlit** for an intuitive graphical user interface (GUI).

---

## 2. What Is YOLO-NAS?
YOLO-NAS is a state-of-the-art object detection model that enhances traditional YOLO models with improved accuracy and efficiency. It is designed for fast real-time inference while maintaining high detection performance.

### **How YOLO-NAS Works:**
- Uses deep learning techniques to detect objects in images and videos.
- Provides **bounding boxes** around detected objects with confidence scores.
- Optimized for high-speed detection without compromising accuracy.

---

## 3. Dataset for Object Detection
The dataset used for training includes various accident scenarios and suspicious activities. Key features include:
- **Accident Detection:** Identifies different levels of accidents (e.g., moderate, severe).
- **Suspicious Activity Detection:** Detects unusual human behaviors that may indicate threats.

---

## 4. Steps for Object Detection Using YOLO-NAS

### **Step 1: Data Preprocessing**
- Load video and image data using `OpenCV`.
- Convert images to a suitable format for YOLO-NAS processing.
- Normalize the data for consistent detection.

### **Step 2: Model Setup**
- Load the **YOLO-NAS** model.
- Set confidence thresholds for accurate detection.
- Define class labels (e.g., moderate accident, severe accident).

### **Step 3: Detection on Images**
- Upload an image via the Streamlit UI.
- Run the **ImageDetection** function from `YOLO.py`.
- Display the processed image with detected objects.

### **Step 4: Detection on Videos**
- Upload a video file or use a live webcam feed.
- Run the **VideoDetection** function from `YOLO.py`.
- Process video frames in real time and overlay detection results.

### **Step 5: Performance Evaluation**
- **Frame Rate (FPS):** Measure processing speed.
- **Bounding Box Accuracy:** Ensure detected objects are correctly classified.
- **Confidence Score:** Optimize model parameters for reliable predictions.

---

## 5. Why Use YOLO-NAS?
- **Real-Time Processing:** Optimized for speed and accuracy.
- **Advanced Deep Learning Architecture:** Provides superior detection performance.
- **Versatile Input Support:** Works with images, videos, and live camera feeds.

---

## 6. Limitations of YOLO-NAS
- **Requires High Computational Power:** Works best with GPUs for real-time inference.
- **Sensitive to Poor Lighting:** Detection accuracy may decrease in low-light conditions.
- **Complex Fine-Tuning:** Requires proper calibration for different environments.

---

## 7. Installation and Setup
### **Prerequisites**
Ensure you have Python 3.x installed.

### **Installation Steps**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo-name.git
   cd your-repo-name
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the application:
   ```bash
   streamlit run app.py
   ```

---

## 8. Usage
- Select the mode (**About App**, **Run on Image**, **Run on Video**).
- Upload an image/video or enable the webcam.
- Adjust confidence levels if necessary.
- View the processed image/video with detected objects.

---

## 9. Future Enhancements
- **Support for Additional Object Detection Models**: Expanding beyond YOLO-NAS.
- **Edge Computing Integration**: Implementing real-time inference on embedded devices.
- **Automated Alert System**: Notifications for detected accidents or suspicious activities.
- **Improved Accuracy**: Utilizing advanced deep learning techniques.

---

## 10. Contributors
- **Heet Gala**
- Saahil Barve
- Akshay Kesarkar

We appreciate contributions from anyone interested in improving this project. Feel free to fork the repository and submit a pull request.

---

## 11. License
This project is licensed under the MIT License.

