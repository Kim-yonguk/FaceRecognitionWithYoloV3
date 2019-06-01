# FaceRecognition Using YoloV3

This program uses Face recognition to blur faces other than specific people in images or videos.
Yolo v3 was used to detect faces in the input. i used yoloface model that was trained to detect face.
And i used Face_recognition to recognition face. 
I used face_recognition from the coordinates of the face obtained through yolo to extract the feature value and compare the stored picture with the feature value.
Then, if the difference is above a certain standard, it is classified as Unknown. And i blurred them using openCV.
I used an opencv tracker in case I couldn't recognize a side face in the video. And I used a movie for voice processing.

## Prerequisites

* dlib
* Face_recognition
* Tensorflow
* opencv-python
* moviepy
* opencv-contrib-python
* Numpy
* imutils
* Keras
* Matplotlib
* Pillow


## Usage

>**Web cam**
```bash
$ python yoloface_gpu.py --video stream
```

>**Videos**
```bash
$ python yoloface_gpu.py --video samples/Filename.mp4
```

>**Images**
```bash
$ python yoloface_img.py --image samples/Filename.jpg
```



## Samples

### Before
<img src =./pic/Before.jpg width="40%" height="40%">

### After
<img src =./pic/After.jpg width="40%" height="40%">


## References

-https://github.com/sthanhng/yoloface
-https://github.com/ageitgey/face_recognition
