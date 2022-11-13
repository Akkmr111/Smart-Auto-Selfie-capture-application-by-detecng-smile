# Smart-Auto-Selfie-capture-application-by-detecng-smile

Everyone loves a smiling picture, so we will develop a project which will capture images every time you smile.
This is a simple machine learning project for beginners and we will use openCV library.

About the Project
What is OpenCV?
OpenCV is an open-source library for computer vision, with a focus on real-time applications.
It focuses mainly on video capture/processing, image processing, and analysis (like face and object detection).
It has many built-in functions and pre-trained models, so we don’t have to worry about training and testing of algorithms.

Project Prerequisites
To implement this project we need to know the following :
1. Basic concepts of Python
2. openCV basics.
To install the library, you can use pip installer from the command line: pip install opencv-python

Download the Source Code for QR Code Generator in Python
Before proceeding ahead, please download selfie project source code and haarcascade XML files using the link:- 

Steps to Develop the Project
Downloading the haarcascade XML files: https://github.com/Akkmr111/Smart-Auto-Selfie-capture-application-by-detecng-smile

For this project, we need haarcascade_frontalface_default.xml and haarcascade_smile.xml files.
Please download these files using the link mentioned in previous step along with the project code.
It is a good programming practice to create separate folders for different files, so make sure you download these files in a separate folder inside project folder.

Haar Cascade:
Haar Cascade is an ML object detection algorithm used to identify objects in an image (treated as a matrix i.e. 2D grid here) or video.
In this algorithm, a cascade function is trained from a lot of positive and negative images which is then used to detect objects in other images.
It can be trained to identify almost any object. In this project, we will be using these pre-trained files. 
The algorithm has four steps:
1. Haar Feature Selection
2. Creating  Integral Images
3. Adaboost Training
4. Cascading Classifiers

Steps Involved to implement Smile Detection and Selfie Capture Project

1. We first import the openCV library.
2. Now start webcam in the second line using the VideoCapture function of cv2.
3. Then, include haarcascade files in the python file.
4. Video is nothing but a series of images so we will run an infinite while loop for the same.
5. Then we are reading images from the video through read().
6. As feature recognition is more accurate in gray images we will convert the image to gray image using cvtColor() and BGR2GRAY which are basic openCV functions.
7. Now we will read faces using an already included haarcascade file and detectMultiscale() function where we pass gray image, ScaleFactor, and minNeighbors.
   ScaleFactor: Parameter specifying zoom image, accuracy depends on it so we will keep it close to 1 but not very close as if we take 1.001(very close to 1),
   then it would detect even shadows so 1.1 is good enough for the face.
   minNeighbors: Parameter specifying how many neighbors each rectangle should have to retain it.
   If it detects a face we will draw an outer boundary of the face using rectangle() method of cv2 containing 5 arguments: image, initial point (x, y),
   an endpoint of principal diagonal (x + width, y + height), color of the rectangular periphery and last parameter is the thickness of drawn rectangular periphery.
   If the face is detected then we will similarly detect a smile and if a smile is detected too we will print Image and save at the location where we want to save them.
	To save the images we will use imwrite() which takes 2 parameters- location and image.
	To break infinite loop, we have used an if statement which becomes true when we press ‘q’ denoting ‘quit’.
	At last, we will release the video.
	Do not forget to destroy all the windows.

Summary:-
In this tutorial, we have developed a python project to detect a smile and capture selfies using openCV.
OpenCV is a popular machine learning library in the field of computer vision and deep learning.
_____________________________________________________________________________________________________________________________________________________________

Other Python Projects:

Face Detecton using Python:- https://www.youtube.com/watch?v=EMLIpRAbRaI&list=PLVO2IRpyPVc0MTmJZSms35tJmCF0_w-nV

GUI Based Scientific Calculator:- https://www.youtube.com/watch?v=6CAuI6YfvSw&list=PLVO2IRpyPVc3m6IkENSqlM171Q9y0g6nn

GUI Based Music player:- https://www.youtube.com/watch?v=kZXg6AIITeY&list=PLVO2IRpyPVc3i-zeBL487cto66rl8eiJY

GUI Based YouTube Video Downloader:- https://www.youtube.com/watch?v=eQLEG4ZUrW8&list=PLVO2IRpyPVc1t1gOQqx4iYYQdPoz5MRP6

GUI Based Digital clock:- https://www.youtube.com/watch?v=-ld7K7L6ues&list=PLVO2IRpyPVc3WcrSWiZ971KKzuEKNtHfL

GUI Based Text Editor:- https://www.youtube.com/watch?v=8dbUCssLJK0&list=PLVO2IRpyPVc1IZxEyhiIOKhXNgaU5VTkT

Virtual Assistant:- https://www.youtube.com/watch?v=UDBH7qKaF5s&list=PLVO2IRpyPVc0to7SQCzZX57EJKHqT4wF5

QR Code Generator and Reader:- https://www.youtube.com/watch?v=iPF3Bn28iVI&list=PLVO2IRpyPVc3uX5-ulmDNT9E7VrO9l4St

_______________________________________________________________________________________________________________________________________________________________

Connect with me:
Facebook:- https://www.facebook.com/ak.kmr
Instagram:- https://www.instagram.com/ak.kmr111/
Email:- akshaydhiman685@gmail.com
_______________________________________________________________________________________________________________________________________________________________
Subscribe:- https://www.youtube.com/channel/UCMsng433EPhAQbgiuQMN-Ig
