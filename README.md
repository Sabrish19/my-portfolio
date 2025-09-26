# Real-Time Face Detection using Yolov8 Project

This repository contains a real-time face detection system built using Python, OpenCV, and YOLOv8 for face detection , Visitercountand visiter entery and Exit . The project identifies unique faces and maintains a database of captured faces.  

---

## Setup Instructions
open in colab:
## Open in Google Colab

You can directly run this project in Google Colab using the following link:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/<sabrish19>/<yolov8>/blob/main/facedetection_Yolov8.ipynb)
or 
copy the code and past it in google colab
1. **Clone the repository**
   ```bash
   git clone https://github.com/<sabrish19>/<yolov8>.git
   cd <yolov8>
2.Create and activate a virtual environment
python -m venv venv
# Windows
venv\Scripts\activate
# Linux/Mac
source venv/bin/activate

3.Install dependencies
pip install -r requirements.txt
4.set up config.json
{
    "camera_id": 0,
    "face_confidence_threshold": 0.6,
    "save_faces": true,
    "faces_folder": "captured_faces",
    "max_active_faces": 50,
    "database_file": "face_database.json"
}

3.Architecture diagram:
https://drive.google.com/file/d/1Sr3w-FR1kSZrsdZbyYnroNkQPQXlzysA/view?usp=sharing

4.Video:

Video Link : https://drive.google.com/file/d/1ecL9BZwJTQtz00M24dAZXdXF7fUDVuL5/view?usp=sharing

This project is a part of a hackathon run by https://katomaran.com
