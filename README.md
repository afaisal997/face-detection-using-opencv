# Face and Eye Detection using OpenCV

This project demonstrates face and eye detection in both real-time (using a webcam) and static images with the help of OpenCV's pre-trained Haar cascades.

## Project Structure
\`\`\`plaintext
├── face_detection_camera.py       # Real-time face detection using webcam
├── face_detection_image.py        # Face detection in an image
├── face_eye_detection_camera.py   # Real-time face and eye detection using webcam
├── face_eye_detection_image.py    # Face and eye detection in an image
├── haarcascade_frontalface_default.xml
├── haarcascade_eye.xml
└── photo.jpg / photo.jpeg         # Sample image for testing
\`\`\`

## Requirements
- Python 3.x
- OpenCV
- Numpy (if needed)

Install the dependencies using:
\`\`\`bash
pip install opencv-python
pip install numpy
\`\`\`

## Usage
### 1. Real-time Face Detection
To perform real-time face detection using your webcam, run:
\`\`\`bash
python face_detection_camera.py
\`\`\`
Press `q` to exit the window.

### 2. Image-based Face Detection
To detect faces in a static image, use:
\`\`\`bash
python face_detection_image.py
\`\`\`
Make sure to replace `photo.jpg` with the name of your image file if different.

### 3. Real-time Face and Eye Detection
For real-time face and eye detection, execute:
\`\`\`bash
python face_eye_detection_camera.py
\`\`\`
Press `q` to exit the window.

### 4. Image-based Face and Eye Detection
To detect both faces and eyes in a static image, run:
\`\`\`bash
python face_eye_detection_image.py
\`\`\`
Ensure `photo.jpeg` is present in the directory.

## Explanation
- **haarcascade_frontalface_default.xml**: This is the pre-trained Haar cascade for frontal face detection.
- **haarcascade_eye.xml**: This is the pre-trained Haar cascade for eye detection.
- **CascadeClassifier**: It is used to load the classifiers for detection.
- **detectMultiScale**: This method detects objects of different sizes in the input image and returns rectangles for each detected object.

## Output
- Blue rectangles represent detected faces.
- Green rectangles represent detected eyes.

# About Project:
The goal of this project is to detect Faces and Eyes in the images and from webcam. I have used Haar feature-based cascade classifiers 
which is one of the effective methods of object detection as proposed by Paul Viola and Michael Jones.

The project contains four python files:

  1. face_detection_image.py 
      
      This file is used to only detect the face of a person from specified image. I had used Elon Musk image if you wants to use another
      image then, make changes at line number 5 in code in place of "elon.jpg" use your image name but, make sure that the image should be 
      at same location where the code is saved.
       
  2. face_detection_camera.py
  
      This file is used to only detect the face of a person from webcam. This code is written for thos who are using inbuilt webcam for
      those how are using external webcam make some changes in code as the line number 4 is "cap = cv2.VideoCapture(0)" make it as
      cap = cv2.VideoCapture(1) i.e. in place of 0 write 1.
      
  3. face_eye_detection_image.py
  
      This file is used to detect the face and eyes of a person from specified image. I had used Elon Musk image if you wants to use another
      image then, make changes at line number 7 in code in place of "elon.jpg" use your image name but, make sure that the image should be 
      at same location where the code is saved.
      
  4. face_eye_detection_camera.py
  
      This file is used to detect the face and eyes of a person from webcam. This code is written for thos who are using inbuilt webcam for
      those how are using external webcam make some changes in code as the line number 5 is "cap = cv2.VideoCapture(0)" make it as
      cap = cv2.VideoCapture(1) i.e. in place of 0 write 1.
      
 # Language and Framework Used:
 
      Language : Python
      Framework : open cv2 (open source computer vision library)
                  For this use command - pip install opencv-python



