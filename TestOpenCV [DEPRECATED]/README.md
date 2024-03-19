Step:
1. sudo nano /etc/apt/sources.list
    1. paste 
       `deb http://archive.debian.org/debian stretch main contrib non-free
       `#deb-src http://archive.debian.org/debian stretch main contrib non-free
       `deb http://archive.ev3dev.org/debian stretch main
       `#deb-src http://archive.ev3dev.org/debian stretch main
2. sudo apt update
3. sudo apt upgrade
4. install the following
    1. `sudo apt install build-essential cmake pkg-config
    2. `sudo apt install (libjpeg-dev) libtiff5-dev (libjasper-dev) libpng-dev
    3. `sudo apt install libavcodec-dev libavformat-dev libswscale-dev libv4l-dev
    4. `sudo apt install libxvidcore-dev libx264-dev
    5. `sudo apt install libfontconfig1-dev libcairo2-dev
    6. `sudo apt install libgdk-pixbuf2.0-dev libpango1.0-dev
    7. `sudo apt install libgtk2.0-dev libgtk-3-dev
    8. `sudo apt install libatlas-base-dev gfortran
    9. `sudo apt install libhdf5-dev libhdf5-serial-dev (libhdf5-103)
    10. `sudo apt install libqt5gui5 libqt5webkit5 libqt5test5 python3-pyqt5
    11. `sudo apt install python3-dev
5. `sudo apt-get install python-opencv
6. `sudo apt-get install python3-opencv
7. `sudo apt-get install python-dev python-numpy
8. `sudo apt-get install python3-dev python3-numpy
9. `sudo apt-get install git
14. `git clone https://github.com/opencv/opencv.git 
15. `mkdir build
16. `cd build
