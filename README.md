# INDIAN-SIGN-LANGUAGE-TO-SPEECH-USING-YOLOv5-WITH-AUDIO-FEEDBACK

This project implements a **ISL to Speech System** using YOLOv5 and LSTM layers to detect **25 Indian Sign Languages**, including **15 words** and **10 numbers**, with an accuracy of **85%**. The system leverages a fine-tuned YOLOv5 model for precise hand detection and LSTM layers for sequence mechanism to enhance recognition performance.

## Output

## Installation

1. **Install YOLOv5**  
   Download the YOLOv5 repository from its official source:  
   ```bash
   git clone https://github.com/ultralytics/yolov5.git
   cd yolov5

2. **Download Required Files**  
   Download the necessary files from the following Google Drive link:  
   [Google Drive](https://drive.google.com/drive/folders/1eVpIyxxl2hf-DfdztyahvSsGvxE__y19?usp=drive_link)  

   After downloading:
   - Extract the 'files.zip'
    - Replace the default `detect.py` file in the YOLOv5 directory with the downloaded `detect.py`.  
     - **Note**: The downloaded `detect.py` includes additional functionality for audio feedback.    
   - Place the trained weights in the `weights/` folder inside the YOLOv5 directory.

4. **Install Dependencies**  
   Navigate to the YOLOv5 directory and install the required dependencies by running:  
   ```bash
   pip install -r requirements.txt

5. **Run the Detection System**  
   Execute the detection system by running the following command in the YOLOv5 directory:  
   ```bash
   python detect.py --weights weights/best.pt --source 0 
