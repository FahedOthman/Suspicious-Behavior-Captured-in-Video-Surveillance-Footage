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
---------------------------------------------------------------
### YOLOv7 :
---------------------------------------------------------------
### Classifier:
#### PreProcessing:
  1. First extract the dataset folder to the same folder as the repository
  2. The `utils` folder contains 3 python scripts to run
  3. run `python utilties/resort_dataset.py`
  4. run `python utilties/create_normal_class.py`
  5. run `python utilties/preprocess.py`

#### Training:
Using `train_set.ipynb` we train the model using this file , a few adjustments is needed in `main()`

We used the Slowfast model with batch size `8`, img_size `224` and frames `25`

#### Testing:
After training the model ,run the `predictions()` giving the video to predict as input

Then it will show what the model has been predicted 

---------------------------------------------------------------
### User Interface:
Navigate to a specific directory: `cd User_Interface`

Then run the command : `streamlit run app.py` 

The UI will open in a Web browser

#### Run Custom Videos:
Open the `Settings.py` file 

Save the video that you want to use in `User_Interface/video`

Then Change the name of `video_1.mp4` for the video that you want ,in the `VIDEO_1_PATH` and `VIDEOS_DICT` code

```python
VIDEO_DIR = ROOT / 'videos' 

VIDEO_1_PATH = VIDEO_DIR / 'video_1.mp4' # Edit here
VIDEO_2_PATH = VIDEO_DIR / 'video_2.mp4' # Edit here
VIDEO_3_PATH = VIDEO_DIR / 'video_3.mp4' # Edit here

VIDEOS_DICT = {
    'video_1': VIDEO_1_PATH, # Edit here
    'video_2': VIDEO_2_PATH, # Edit here
    'video_3': VIDEO_3_PATH, # Edit here
}


```



---------------------------------------------------------------
## References :
YOLO v7: https://github.com/WongKinYiu/yolov7

Classifier : https://github.com/LeadingIndiaAI/Armed-Injured-and-other-Suspicious-Activity-Recognition-using-Drone-Surveillance

User Interface: https://github.com/CodingMantras/yolov8-streamlit-detection-tracking
