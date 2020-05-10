# Yolov3-Object-Detection-with-CPU-or-GPU

Real-time object detection using opencv with Yolo model.

### Download Yolov3 weights

Open terminal and run:
```
mkdir weight
cd weight
wget https://pjreddie.com/media/files/yolov3.weights
```
### How to Run

For image:

`python yolov3_image.py`

For webcam/RTSP stream:

`python yolov3_video.py`


To use GPU:
before running with GPU make sure openv build with cuda
```
net.setPreferableBackend(cv2.dnn.DNN_BACKEND_CUDA)
net.setPreferableTarget(cv2.dnn.DNN_TARGET_CUDA)
```
