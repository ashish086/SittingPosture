# Lateral Sitting Posture Detection using YOLOv5

### Built With

![Python]

# Getting Started

### Prerequisites

* Python 3.9.x

### Installation  
If you have an NVIDIA graphics processor, you can activate GPU acceleration by installing the GPU requirements. Note that without GPU acceleration, the inference will run on the CPU, which can be very slow.  
#### Windows  
  
1. `git clone https://github.com/ashish086/SittingPosture.git`  
2. `python -m venv venv`  
3. `.\venv\scripts\activate.bat`  
##### Default/NVIDIA GPU support:  
4.  `pip install -r ./requirements_windows.txt` **OR** `pip install -r ./requirements_windows_gpu.txt`

### Run the program

`python application.py <optional: model_file.pt>` **OR** `python3 application.py <optional: model_file.pt>`

The default model is loaded if no model file is specified.

# Model
The program uses a custom trained [YOLOv5s](https://github.com/ultralytics/yolov5/blob/79af1144c270ac7169553d450b9170f9c60f92e4/models/yolov5s.yaml) model that is trained on about 160 images per class for 146 epochs. The model has two classes: sitting_good and sitting_bad to give feedback about the current sitting posture.
