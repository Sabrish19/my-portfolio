# Real-Time Face Detection using Yolov8 Project

This project is a real-time face detection and recognition system built using Python, YOLOv8, and DeepFace.  
It detects faces from a webcam, checks if the face is already in the database, and counts the number of  visitors.

---

## Setup Instructions
open in colab:
## Open in Google Colab

You can directly run this project in Google Colab using the following link:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Sabrish19/yolov8/blob/main/facedetection_Yolov8.ipynb)
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

4.## How This Project Works

   1. **Start Webcam**  
   - The system uses your webcam to capture live video.

   2. **Detect Faces**  
   - YOLOv8 detects faces in real time and shows them on the screen.

   3. **Recognize Faces**  
   - Each detected face is compared with a database of existing faces.

   4. **Check Visitor**  
   - If the face is already in the database → marked as **“Existing Visitor”**.  
   - If the face is new → marked as **“Unique Visitor”**, stored in the database, and visitor count increases.

   5. **Show Results on Camera**  
   - **Green box** → Unique visitor.  
   - **Red box** → Existing visitor.  
   - Shows the **total number of unique visitors** on the screen.

   6. **Configuration**  
   - You can set camera ID, detection confidence, and database file in `config.json`.  
   - Example `config.json`:

5.set up config.json
{
    "camera_id": 0,
    "face_confidence_threshold": 0.6,
    "save_faces": true,
    "faces_folder": "captured_faces",
    "max_active_faces": 50,
    "database_file": "face_database.json"
}

6.Architecture diagram:
https://drive.google.com/file/d/1Sr3w-FR1kSZrsdZbyYnroNkQPQXlzysA/view?usp=sharing

7.Video:

Video Link : https://drive.google.com/file/d/1ecL9BZwJTQtz00M24dAZXdXF7fUDVuL5/view?usp=sharing

This project is a part of a hackathon run by https://katomaran.com
