## Real-Time_Person_Detection_and_Tracking
This project uses OpenCV to connect to an RTSP video stream, process object tracks, and interactively select a bounding box with a mouse click. A timer is displayed for the selected bounding box, even if the detection is skipped for a few frames.

## Features
- Connect to an RTSP stream (e.g., from the IP Webcam app on Android).
- Process object tracks and displays bounding boxes.
- Click on a bounding box to select it, change it to Red, and start a timer.
- Display the timer on the selected bounding box.
- Maintain the selected bounding box for a specified grace period if detection is skipped.

## Prerequisites
- Python
- OpenCV
- Ultralytics
- IP Webcam app (or any RTSP video streaming camera)

## Installation

1. **Clone the repository**:
    ```bash
    git clone git clone https://github.com/SohailWarraich/Real-Time_Person_Detection_and_Tracking.git
    cd Real-Time_Person_Detection_and_Tracking_using_YOLOv8
    ```

2. **Install dependencies**:
    ```bash
    pip install opencv-python-headless
    pip install ultralytics
    ```

3. **Install and configure the IP Webcam app**:
    - Download and install the IP Webcam app from the Google Play Store.
    - Open the app, configure settings, and start the server.
    - Note the IP address and port displayed by the app.

## Usage

1. **Modify the RTSP URL**:
    - In `main_script.py`, set the `rtsp_url` variable to match the IP address and port of your IP Webcam app:
      ```python
      rtsp_url = 'rtsp://<IP_ADDRESS>:<PORT>/h264_ulaw.sdp'
      ```

2. **Run the script**:
    ```bash
    python main.py
    ```

## File Structure

- `main.py`: Main script to capture RTSP stream, process frames, and display the video.
- `utilis.py`: Contains the `TrackProcessor` class for handling track processing and timer functionality.
- `README.md`: Documentation of the code.
### Visualize Input and Output Result
![frame1](https://github.com/SohailWarraich/Real-Time_Person_Detection_and_Tracking/blob/main/screenshort/frame1.png)

![frame2](https://github.com/SohailWarraich/Real-Time_Person_Detection_and_Tracking/blob/main/screenshort/frame2.png)


For any questions or issues, please contact [arshadsohail092@gmail.com](arshadsohail092@gmail.com).

