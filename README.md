# Driver-Drowsiness-Detection
Drowsy driver detection with OpenCV and Dlib for eye and yawn detection. Alarm as well as sms alert integrated.

Create an account on twilio and get account ID and authorized token. Replace them in the python file accordingly. 
Also replace the from number in lines 133 and 162 with the number provided by twilio. 
In lines 134 and 163, replace the number with the number of the emergency contact.

To run the detection system install anaconda prompt. Navigate to the folder where the repository is saved and execute the following commands on anaconda.

conda create --name opencv-env python=3.8
activate opencv-env
pip install numpy scipy matplotlib scikit-learn jupyter imutils playsound os geocoder twilio
pip install opencv-contrib-python
conda install -c conda-forge dlib

Now the file should execute smoothly with the command:
python detect_drowsiness.py --webcam 0 --alarm alarm.wav
