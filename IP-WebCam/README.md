# IpWebCam-FacialRecognition
Script For Demonstrating the Beauty and Simplicity OF Facial Recognition API Using Ip WebCam App

## Getting Started
Here, I use the **Facial Recognition** API with **IP Webcam** App for Android to achieve **Real Time Wireless Face Detection**.

## Dependinces
We will need some libraries installed to start:

````
pip3 install numpy face_recognition opencv-python --user
````

## Testing
All you need now is to run the python script and see the magic happens, but first you will need to install the ip WebCam app on your android phone and start it to acquire the ip address and port number (usually: 8080) of the transmission and then you just need to type this on your command line:

```
python3 ip_webcam_face_recognition.py <ip address>
```

**Replace `<ip address>` with the acquired ip with the port from the app**

Example:

- ip_address: **192.168.1.1:8080**

and you should see what your phone sees and identify the photos of sisi & mubark .... wait WHAT?!

## How It Works ?

Now the script dose 3 things exactly:

1. it goes to the folder `Training_images` and loop over the images inside of it to acquire the names and photos of the persons you want to identifiy
2. it gets the frames from the ip Webcam App and transform it to a working numpy/openCV format
3. it makes the predictions and highlight them by rectangles around the faces in the video.

Simple right :)

## How to use it ?

Now, this should be simple as i demonstrated above with the code but there is some stuff i want to add here

1. you can specifiy another folder with the training faces on it by typing `-p <Training_faces folder path>` after the initial running command
2. you can train the script on your images by putting a clear photo of you in the training_images folder with your name on it
3. you can even access your phone from another country via the internet using something called **PortForwarding** 
