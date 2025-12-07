
# OBJECT DETECTION 
📌**Project overview:**
This project focuses on developing a real-time object detection system using OpenCV and a pre-trained object detection model. The system captures video frames either from a video file or a live webcam feed, processes each frame, and identifies various objects within the scene.

The project demonstrates how computer vision techniques can automatically detect and classify objects in real time, making it useful for applications such as surveillance, robotics, traffic monitoring.

📌**Key Features:**
---
1.**Real-Time Video Processing**-->

The system reads frames continuously from:

A pre-recorded video, OR from webcam.

Each frame is processed instantly to detect objects.
 
**How To open our laptop cam for check?**

There is nothing to worry about ,it here when we try to read the **cv2.VideoCapture()** if we just write this then it will fail to access the video as no source is given and as you can see in my code.

cap=cv2.VideoCapture()

if not cap.isOpened():

    cap = cv2.VideoCapture(0)


Meaning: The cap can't be openede now so this make this statemebnt true and it will access your webcam.

**2. Object Detection Using Pre-Trained Model:**

My code uses model.detect() to find objects,

Returning class indices, confidence scores, and bounding boxes.

This allows the model to detect objects like:

Person,
Car,
Do,
Chair,
And other COCO dataset classes (up to 80 classes).

**3. Bounding Boxes & Labels:**

For each detected object:

A bounding box is drawn around it.

The class name is printed on top of the box.

Confidence threshold: 0.55, ensuring only reliable detections are shown.

Example steps inside your code:

cv2.rectangle() -->draws the box

cv2.putText()--> writes label + confidence

Objects appear marked in red for clarity.
**BGR**--->

**(255,0,0)---->Blue**

**(0,255,0)---->Green**

**(0,0,255)---->Red**

**4. Live Display Window:**

Using:

cv2.imshow("Object Detection in Video", frame)


My model displays annotated frames in a pop-up window.
It updates continuously until the user presses Q.

**5.Image detection:**

It can also Implemented in image as i show in my code,
using **cv2.rectangle()** ,it can show which one is cat,person or any keyword present in the coco text.

## 🔗 Links:
--
**Link1:**

https://github.com/opencv/opencv/wiki/TensorFlow-Object-Detection-API
--------> **official opencv github account**,froze_interface_graph

**Link2:** 
https://github.com/pjreddie/darknet/blob/master/data/coco.names ------>coco data sets

**Link3:** https://gist.github.com/dkurt/54a8eb51beb3bd3f770b79e56927bd7
----->for configuration file

**📌 Required Libraries:**
--
Install the following Python libraries before running the project:

pip install opencv-python

pip install matplotlib

pip install numpy

**or**

**You can use:**  pip install numpy matplotlib opencv-python




**📌Modules Used Here:**
--
1.**cv2**

2.**matplotlib.pyplot**

3.**numpy**

   ---------------------------Nothing more than this .


## **🔗 Project Video Demo:**

https://github.com/user-attachments/assets/35c20578-229f-4c37-bc83-2386720af1d1

