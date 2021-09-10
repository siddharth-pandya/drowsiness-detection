# drowsiness-detection
Application can detect drowsiness and raise alarm.

NOTE: We will create and work in VIRTUAL ENVIRONMENT and install all dependencies so as to prevent affect on root directory

open windows 'cmd' typing cmd in search (not conda command window) as an administrator

Download and install python if not pre-existing

check python version> python -V
Install virtual environment> pip install virtualenv
test installation> virtualenv --version

Use the drowsiness_main.py file and the alarm file and put them in one directory, and download and add a pre-existing file named shape_predictor_68_face_landmarks.dat.
Now change the directory to 'Drowsiness_detection' folder (at this type your command prompt window should look like C:\Drowsiness_detection>)

create virtual environment repositery>virtualenv env (this will create a folder with name 'env' inside working reositery 'Drowsiness_detection')
Run the command to activate virtual environment>env\Scripts\activate

(after successful run, cmd window will look like '(env) C:\Drowsiness_detection>' means you have successfully created and activated virtual env and ready to work)

Install necessary packages
(env) C:\Drowsiness_detection>pip install --upgrade imutils
(env) C:\Drowsiness_detection>pip install playsound
(env) C:\Drowsiness_detection>pip install pyobjc
(env) C:\Drowsiness_detection>pip install scipy
(env) C:\Drowsiness_detection>pip install dlib
(env) C:\Drowsiness_detection>pip install opencv-python
(env) C:\Drowsiness_detection>pip install dlib
########## NOW YOU ARE READY To Test SCRIPT ##############################

(env) C:\Drowsiness_detection>python detect_drowsiness.py --shape-predictor shape_predictor_68_face_landmarks.dat
If you want to save alarm audio file run following command

17)(env) C:\Drowsiness_detection>python detect_drowsiness.py --shape-predictor shape_predictor_68_face_landmarks.dat --alarm alarm.wav

REFERENCES: https://www.ee.ryerson.ca/~phiscock/thesis/drowsy-detector/drowsy-detector.pdf
