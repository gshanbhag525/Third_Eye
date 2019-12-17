# Third_Eye
----------
## Demonstration 
[Third Eye: a Remote Surveillance System](https://www.youtube.com/watch?v=p-T-LUWfCaY)

![](images/image1.JPG)
### Server

This app is built based on Django.

Control the Smart Video Vehicle via the gravity sensor on a cell phone - control the car and the camera onside,
as well as view the camera video in real time. What's more, on the app, 
you can conveniently calibrate the car turning and the pan-tilt. 

The Android app project files are under Android_App folder.

This server runs on Raspberry Pi, and is controlled by the Android app.

#### Setup:
1. Install Django:

	 sudo pip install django
	 
2. Then, at `Third_Eye/http_server/` run:

	`sudo python manage.py runserver 0.0.0.0:8000`

3. Open the app on your phone, and type in your Raspberry Pi's IP address,

   	click FORWARD (the right arrow) and then you can see the image from the car's camera.

#### Calibration:
Begin calibration by clicking on the dot in a circle at the corner. 
Note: the calibration steps are quite small. For convenience, you can click more times or even type in a specific value.

#### Control:
 - Control the car direction by tilting your phone, like a steering wheel.
 - Control the car forward/backward by the up/down arrow on the left.
 - Control the camera pan/tilt by the up/down/left/right arrow on the right, 
   And set the camera back to the default position by the middle dot.
 - Change the motor speed by the bar under the camera view

### App:
1. App using AppInventer:

The Android app is build under [MIT App Inventor 2](http://ai2.appinventor.mit.edu/),
so no detail source code, just a project folder, which you can edit it with App Inventor 2. 
The project files are under html_server/Android_App folder.

2. App using Android Studio:

The Android app is built using android studio .
The project files are under project_files/Controller folder.
