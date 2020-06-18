# movementDetector
This code is based on a [tutorial by PyImageSearch](https://www.pyimagesearch.com/2015/06/01/home-surveillance-and-motion-detection-with-the-raspberry-pi-python-and-opencv/) on building a motion detection system for the Raspberry Pi with background subtraction.

## Hardware
This code ran on/with:
- Raspberry Pi 3 B+
- NoIR (No InfraRed) camera
- Official power supply by Raspberry providing 5.1V and 2.5A

## OS
The Raspbian version installed on the Raspberry Pi can be seen by checking the output of `cat /etc/os-release`:
```
PRETTY_NAME="Raspbian GNU/Linux 10 (buster)"
NAME="Raspbian GNU/Linux"
VERSION_ID="10"
VERSION="10 (buster)"
VERSION_CODENAME=buster
ID=raspbian
ID_LIKE=debian
HOME_URL="http://www.raspbian.org/"
SUPPORT_URL="http://www.raspbian.org/RaspbianForums"
BUG_REPORT_URL="http://www.raspbian.org/RaspbianBugs"
```

## How to use
Follow the instructions provided by the PyImageSearch link provided above. These will create a Python virtual environment with all the needed packages. Whenever you want to run the code, you will have to activate this virtual environment and finally launch:
```
python pi_surveillance.py -c conf.json
```

Note that the the conf.json file needs to be edited with the correct Dropbox token and URL to save the images.

## Sample results
Images of Mika eating her treat sneakily after hiding under the blanket in a fully dark room can be found in the `sampleResultImages` directory.

![alt text](https://github.com/BourbonCreams/movementDetector/blob/master/sampleResultImages/Wednesday%2017%20June%202020%2005:08:17PM.jpg?raw=true)

## VNC (Virtual Network Computing)
If you want to use VNC to run the application on a remote desktop, you have to enable VNC on the Raspberry Pi (run `sudo raspi-config`) and then follow the instructions on the official [Raspberry page for VNC](https://www.raspberrypi.org/documentation/remote-access/vnc/), which will ask you to install the VNC viewer on your desktop.
Once logged in, remember to enable the virtual environment and then launch the application as described above.
