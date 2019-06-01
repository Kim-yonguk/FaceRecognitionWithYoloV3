# FaceRecognition Using YoloV3

This program uses Face recognition to blur faces other than specific people in images or videos.
Yolo v3 was used to detect faces in the input. i used yoloface model that was trained to detect face.
And i used Face_recognition to recognition face. 
I used face_recognition from the coordinates of the face obtained through yolo to extract the feature value and compare the stored picture with the feature value.
Then, if the difference is above a certain standard, it is classified as Unknown. And i blurred them using openCV.
I used an opencv tracker in case I couldn't recognize a side face in the video.
