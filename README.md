# movementDetector
This code is based on a [tutorial by PyImageSearch](https://www.pyimagesearch.com/2015/06/01/home-surveillance-and-motion-detection-with-the-raspberry-pi-python-and-opencv/) on building a motion detection system for the Raspberry Pi with background subtraction.

# Hardware
This code ran on/with:
- Raspberry Pi 3 B+
- NoIR (No InfraRed) camera
- Official power supply by Raspberry providing 5.1V and 2.5A

# How to use
Follow the instructions provided by the PyImageSearch link provided above. These will create a Python virtual environment with all the needed packages. Whenever you want to run the code, you will have to activate this virtual environment and finally launch:
```
python pi_surveillance.py
```

Note that the the conf.json file needs to be edited with the correct Dropbox token and URL to save the images.

# Sample results
Images of Mika eating her treat sneakily after hiding under the blanket in a fully dark room can be found in the `sampleResultImages` directory.

![alt text](https://github.com/BourbonCreams/movementDetector/blob/master/sampleResultImages/Wednesday%2017%20June%202020%2005:08:17PM.jpg?raw=true)
