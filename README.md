# 🎯 AI Object Detection & Tracking

An AI-powered computer vision application that detects, tracks, and counts objects in real time using **YOLO, OpenCV, and Python**. The project supports image, video, and webcam input through a simple Streamlit web interface.

## 📌 Table of Contents

- [About the Project](#-about-the-project)
- [Problem Statement](#-problem-statement)
- [Solution](#-solution)
- [Key Features](#-key-features)
- [How It Works](#-how-it-works)
- [Technology Stack](#-technology-stack)
- [Project Structure](#-project-structure)
- [Installation and Setup](#-installation-and-setup)
- [How to Use](#-how-to-use)
- [Applications](#-applications)
- [Future Improvements](#-future-improvements)
- [Author](#-author)

---

## 📖 About the Project

AI Object Detection & Tracking is a computer vision project that uses the YOLO object detection model to identify objects in images and video streams.

In addition to detecting objects, the application tracks individual objects across video frames and assigns unique tracking IDs. It also displays bounding boxes, object labels, and object counts to help users understand what is happening in a scene.

The project provides an accessible interface through Streamlit, allowing users to interact with the detection system without needing to use command-line tools for every operation.

## ❗ Problem Statement

Manually identifying and tracking multiple objects in images or video footage can be time-consuming and difficult. Traditional approaches may struggle to process video efficiently or maintain object identities across consecutive frames.

An automated solution is needed to detect objects, track their movement, and display useful information in an understandable format.

## 💡 Solution

This project combines YOLO-based object detection with OpenCV video processing and tracking capabilities.

The application processes image, video, or webcam input, detects objects, displays their locations, and uses tracking IDs to distinguish objects across video frames.

A Streamlit interface makes these capabilities easier to access and use.

## ✨ Key Features

- **Real-Time Object Detection:** Detect objects in webcam streams.
- **Multi-Object Tracking:** Track multiple objects across video frames.
- **Unique Tracking IDs:** Assign IDs to distinguish tracked objects.
- **Bounding Boxes:** Visually highlight detected objects.
- **Class Labels:** Display the predicted class of each object.
- **Object Counting:** Show the number of detected objects.
- **Adjustable Confidence Threshold:** Control the confidence level used to display detections.
- **Image Detection:** Analyze uploaded images.
- **Video Detection:** Process video files for detection and tracking.
- **Streamlit Web Interface:** Interact with the application through a browser-based interface.

## ⚙️ How It Works

1. **Input:** The user selects a webcam stream, image, or video.
2. **Frame Processing:** OpenCV handles image and video processing.
3. **Object Detection:** The YOLO model identifies objects and predicts their classes and locations.
4. **Object Tracking:** The tracking functionality maintains object identities across video frames.
5. **Visualization:** Bounding boxes, class labels, tracking IDs, and counts are displayed.
6. **User Interaction:** The Streamlit interface lets users access the available detection features.

### 🔄 Workflow

```text
User Input
    |
    v
Image / Video / Webcam
    |
    v
OpenCV Processing
    |
    v
YOLO Object Detection
    |
    v
Object Tracking
    |
    v
Tracking IDs and Object Counts
    |
    v
Display Results in Streamlit
```

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| YOLO | Object detection |
| Ultralytics | YOLO model and tracking interface |
| OpenCV | Image and video processing |
| PyTorch | Deep learning framework used by the model |
| Streamlit | Web-based user interface |
| Computer Vision | Image and video analysis |

## 📂 Project Structure

```text
Object_Detection_Project/
│
├── app.py              # Main application
├── web_app.py          # Streamlit web interface
├── requirements.txt    # Python dependencies
├── README.md           # Project documentation
├── .gitignore          # Files excluded from Git
└── venv/               # Local virtual environment (not committed)
```

*Note: The exact responsibilities of `app.py` and `web_app.py` depend on their implementation in your repository.*

## 🚀 Installation and Setup

### Prerequisites

Before starting, make sure you have:

- Python installed on your computer.
- Git installed.
- A code editor such as Visual Studio Code.
- A webcam if you want to use live detection.
- The project files cloned or downloaded from GitHub.

### Step 1: Clone the Repository

Replace `YOUR-GITHUB-USERNAME` with your GitHub username if the repository URL differs.

```bash
git clone https://github.com/YOUR-GITHUB-USERNAME/Object_Detection_Project.git
```

Navigate to the project directory:

```bash
cd Object_Detection_Project
```

### Step 2: Create a Virtual Environment

```bash
python -m venv venv
```

### Step 3: Activate the Virtual Environment

**Windows PowerShell:**

```powershell
.\venv\Scripts\Activate.ps1
```

**Windows Command Prompt:**

```cmd
venv\Scripts\activate.bat
```

### Step 4: Install Dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

If PyTorch or other model dependencies fail to install, check the official installation instructions for your operating system and hardware.

### Step 5: Start the Application

If `web_app.py` contains the Streamlit interface, run:

```bash
streamlit run web_app.py
```

If `app.py` is the Streamlit entry point in your implementation, use:

```bash
streamlit run app.py
```

Open the local URL displayed in the terminal to access the application.

## 🖥️ How to Use

1. Start the application using the appropriate Streamlit command.
2. Open the local web address shown in your terminal.
3. Select the supported input type: image, video, or webcam.
4. Upload an image or video, or enable webcam detection as supported by the interface.
5. Adjust the confidence threshold if the application provides that setting.
6. View the detected objects, bounding boxes, class labels, tracking IDs, and object counts.
7. Review the processed results in the application.

## 🌍 Applications

Object detection and tracking can be useful in several areas:

- **Smart Surveillance:** Detect and track objects in monitored environments.
- **Traffic Monitoring:** Analyze vehicles and traffic movement.
- **Retail Analytics:** Count and observe objects in retail environments.
- **Robotics:** Help robots perceive objects in their surroundings.
- **Industrial Automation:** Support visual inspection and object monitoring.
- **Computer Vision Learning:** Explore practical applications of AI and deep learning.

These are potential applications of the underlying technology, not claims that every use case is implemented in this project.

## 🔮 Future Improvements

Possible enhancements include:

- Save processed videos and annotated images.
- Add object-specific counting.
- Display detection statistics and charts.
- Improve tracking stability in crowded scenes.
- Add support for selecting different YOLO models.
- Provide downloadable detection results.
- Improve the interface for mobile and desktop users.
- Optimize performance for different hardware configurations.

## 🎓 Learning Outcomes

Through this project, developers can gain practical experience with:

- Python application development.
- Deep learning and computer vision.
- YOLO-based object detection.
- Video frame processing using OpenCV.
- Multi-object tracking concepts.
- Building interactive applications with Streamlit.
- Managing project dependencies and Git repositories.

## 👩‍💻 Author

**Reema Dsouza**

GitHub: [@reemadsouza2006-dev](https://github.com/reemadsouza2006-dev)

---

⭐ If you find this project interesting, consider starring the repository!

*Developed as a practical project in AI and Computer Vision.*
