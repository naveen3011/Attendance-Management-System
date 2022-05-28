
# Facial Recognition Engage2022
## Attendance-Management-System

**Problem Statement :** <br>
Face Recognition  *(To develop a browser-based application to demonstrate the application of Face Recognition technology).*

## Objective
Nowadays everyone wants that technology can help them to make them work easily. So , I made one  project which can help to take attendance so easily without any paperwork.


![GitHub Logo](https://github.com/naveen3011/Attendance-Management-System/blob/main/photo/face-REC..png)
<p align="center">
    Face Recognition
</p>


**Solution :** <br>
The purpose of this project is to take attendance using face detection. This program makes the CSV files of present attendees automatically After successful face detection. Also, It will make a CSV file for registered students’ info.

**Domain :** <br>
AI/ML and Computer-Vision.<br>
*Face Recognition application is developed in python language using these libraries. OpenCV, Numpy, OS, Pandas, Tkinter.*

## Flow chart 
![Flow chart](https://github.com/naveen3011/Attendance-Management-System/blob/main/photo/flowchat.png)<br>


## How to run?
First of all, simply [download](https://github.com/naveen3011/Attendance-Management-System) this repo and install all the dependencies required for running this application from **[requirements.txt](https://github.com/naveen3011/Attendance-Management-System/blob/main/requirements.txt)**.

Open the terminal and run the following command *(Make sure you are connected to internet)*<br>K
`pip install -r /requirements.txt`

OR<br>
If you don't have required laibreries then firat you need to install that.

OpenCV
>pip install OpenCV-python

Numpy
>pip install numpy

Pandas
>pip install pandas

Os 
>pip install os

Tkinter 
>pip install tkinter

DateTime
>pip install DateTime

Now For run this project you need [haarcascade_frontalface_default.xml](https://github.com/naveen3011/Attendance-Management-System/blob/main/haarcascade_frontalface_default.xml) along with this [python file](https://github.com/naveen3011/Attendance-Management-System/blob/main/main.py) which contains the haar cascade features of a face.
Now you are good to go. 


Once all the dependencies are installed, now your system is ready to **run** this application 🥳<br>
Just open [main.py](https://github.com/naveen3011/Attendance-Management-System/blob/main/main.py) on your IDE(VS Code) & **right-click** there and click on **'Run Python File in Terminal'** *as shown below...*


![ide image](https://github.com/naveen3011/Attendance-Management-System/blob/main/photo/1.png)<br>
![Output](https://github.com/naveen3011/Attendance-Management-System/blob/main/photo/2.png)
<p align="center">
    Final Output
</p>
<br>


## I’m going to explain my whole project in 4 parts.

# Part 1: GUI
In this project, I made  simple GUI using the python Tkinter library so that the user can easily use this project without any backend knowledge. Tkinter is the standard GUI library for Python.

For making this GUI I mainly used Tkinter’s frame, menubar, button, label, message box, table, textbox, etc. I divide my main screen into two parts which are nothing but frames. one is for Registration and the second is for taking attendance.

![GUI](https://github.com/naveen3011/Attendance-Management-System/blob/main/photo/2.png)
<p align="center">
    GUI
</p>
<br>
As shown in the above image this GUI will help users to register new students as well as to take attendance. At the bottom, it will also show you the total number of registered students.
<br>
This GUI window also contains menubar with two sub-menus Help and About. The help menu contains 3 commands contact me, change Admin Password, exit.<br>

![GUI](https://github.com/naveen3011/Attendance-Management-System/blob/main/photo/3.png)
<p align="center">
    Change Admin Password
</p>
<br>


## Part 2:Take Images

when users register for new students it will take 100 images of that student and save these images to one folder which will be created at the time of first registration. I use OpenCV to take images and detection.

OpenCV is a library of programming functions mainly aimed at real-time computer vision. I used a cascade classifier of OpenCV for face detection. To use this cascade classifier we need the haarcascade_frontalface_default.xml file which includes all the haar cascade features of a face.

![GUI](https://github.com/naveen3011/Attendance-Management-System/blob/main/photo/4.png)
<p align="center">
    Taking Images of Student
</p>
<br>
When users want to register new students they have to enter first details like ID and Name. After that, they have to take images of the student that when the user presses the button ‘Take Images’ the webcam will start and it will take 100 images of the student.<br>

There are some methods in OpenCV to take Images. using video frames of OpenCV I’m taking frames and from that, I’m extracting only face images using a cascade classifier. After taking images I will store those images in one folder.

## Part 3: save Profile
When images will be taken for any student user needs to click the ‘save profile’ button so that it will ask for the admin password. If the admin password was not set it will ask you first to set the admin password or else you need to enter the admin password. This password will be saved in one plan txt file.<br>
If this password is correct then it will call the trainer function which will be going to generate a YML file and it will train our LBPH recognizer using those 100 images. This YML file and password txt file will save in one different folder named “pass_train”.<br>
After saving the profile there are 3 different folders generated in the current directory. Out of that 3 folders, one is containing images of students, the second one is containing a CSV file of students’ details and the third one is containing a pass.txt file and YMLfile.<br>
![GUI](https://github.com/naveen3011/Attendance-Management-System/blob/main/photo/7.png)
<p align="center">
    After saving profile
</p>
<br>
## Part 4:Taking attendance

When a user wants to take attendance and press the ‘take attendance’ button webcam will start and one video frame window will generate to recognize the faces using the YML file. If the face will successfully recognize then it will put the name of the person at the bottom of the rectangle which is showing the detected face area.
![GUI](https://github.com/naveen3011/Attendance-Management-System/blob/main/photo/6.png)
<p align="center">
   Taking Attendance
</p><br>



# Checkout this [YouTube link](https://youtu.be/mYZvIkMlNCA) for breif explanation, Thankyou❤
