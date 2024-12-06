# NeuroDetect - Object Detection using YOLOv8 and Streamlit

A streamlined application for object detection and tracking using YOLOv8, integrated with an interactive dashboard powered by Streamlit. This project combines cutting-edge object detection algorithms with an intuitive interface to provide real-time analytics for images and videos.

---

## 📖 About the Project

### Problem Statement
Object detection and tracking are critical components in computer vision with applications ranging from surveillance systems to industrial automation. However, existing tools often lack user-friendly interfaces and require significant technical expertise to operate.

### How This Project Solves It
This project offers:
1. **Ease of Use**: A clean, intuitive dashboard for uploading videos or images, selecting object classes to detect, and visualizing results.
2. **Real-Time Analytics**: Displays detection results, including bounding boxes, class labels, and counts.
3. **Interactivity**: Provides options to download detection data for further analysis, making it ideal for users without extensive technical knowledge.

---

## 🚀 How to Run the Project

### Prerequisites
Ensure the following are installed on your system:
- Python 3.8+
- Streamlit
- OpenCV
- Ultralytics (YOLOv8)
- Plotly
- PIL

Steps to Run
Clone the repository:
bash
Copy code
git clone https://github.com/your-username/computer-vision-dashboard.git
cd computer-vision-dashboard
Launch the Streamlit app:
bash
Copy code
streamlit run app.py
Access the app in your browser at http://localhost:8501.
🛠 How the Project Works
About Section:

Explains the purpose of the project and its functionalities.
Includes an autoplay video or GIF showcasing the application.
Video Mode:

Upload a video file.
Select object classes and confidence threshold from the sidebar.
View detections in real-time, with bounding boxes drawn on detected objects.
Download detection data as a CSV file for further analysis.
Image Mode:

Upload an image file.
Perform object detection for selected classes.
Visualize results directly on the dashboard.
Dashboard Features:

Real-time visualizations of detected objects.
Interactive charts and download options for detection statistics.
💡 Challenges Faced and How We Overcame Them
Video Playback Issues:

Initially faced problems with autoplay functionality for embedded videos. Resolved by converting the demo video to a GIF and using st.image for seamless playback.
Handling Large Files:

Uploading large videos/images caused performance lags. Mitigated this by resizing input files dynamically using OpenCV.
Real-Time Detection Rendering:

Streamlit's default rendering posed challenges for displaying real-time detections. Solved this by leveraging Streamlit's st.image and efficiently updating frames.
Data Storage and Management:

Managing detection data for multiple runs required a structured approach. Addressed by using temporary JSON files for intermediate storage and ensuring clean-up post-inference.
🌟 Future Enhancements
Add support for additional object detection models.
Enable real-time webcam feed for live detections.
Expand analytics capabilities with more advanced visualization tools.
