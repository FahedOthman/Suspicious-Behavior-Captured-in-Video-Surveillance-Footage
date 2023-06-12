# Suspicious-Behavior-Captured-in-Video-Surveillance-Footage
Detection of Suspicious Behavior Captured in Video Surveillance Footage Using Deep Learning

### Dataset used :
 https://www.kaggle.com/mateohervas/dcsass-dataset   
 Delete the second DCSASS Dataset folder and Labels folder
 
### Clone the Repository:
https://github.com/FahedOthman/Suspicious-Behavior-Captured-in-Video-Surveillance-Footage.git

### Requirments:
Download the Requirements.txt file 

`pip install -r Requirements.txt`
### YOLOv7 :
### Classifier:
### User Interface:
Navigate to a specific directory: `cd User_Interface`

Then run the command : `streamlit run app.py` 

The UI will open in a Web browser

Then Change the name of `video_1.mp4` for the video that you want ,in the `VIDEO_1_PATH` and `VIDEOS_DICT` code
### Run Custom Videos:
Open the `Settings.py` file 

Save the video that you want to use in `User_Interface/video`
```python
VIDEO_DIR = ROOT / 'videos' 

# Edit here
VIDEO_1_PATH = VIDEO_DIR / 'video_1.mp4' 
VIDEO_2_PATH = VIDEO_DIR / 'video_2.mp4'
VIDEO_3_PATH = VIDEO_DIR / 'video_3.mp4'

# Edit here
VIDEOS_DICT = {
    'video_1': VIDEO_1_PATH,
    'video_2': VIDEO_2_PATH,
    'video_3': VIDEO_3_PATH,
}


```




## References :
YOLO v7: https://github.com/WongKinYiu/yolov7

Classifier : https://github.com/LeadingIndiaAI/Armed-Injured-and-other-Suspicious-Activity-Recognition-using-Drone-Surveillance

User Interface: https://github.com/CodingMantras/yolov8-streamlit-detection-tracking
