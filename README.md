# MVP_Disk_Image
Image file of the MVP SD Card

This is the SD card pulled from my MVP, run through Win32 Disk Imager, then through 7-Zip to make the zip file.
You should be able to use Etcher to https://drive.google.com/drive/folders/0B-63rlluTVV5dHBxQWROM29MNUk?usp=sharingextract the image to an SD card (32G suggested) and then have a complete MVP software environment.
You are left to connect to the internet.

This first version is a quick and dirty version to meet user needs, and will likely be tested and polished more in the future.

NOTE: the MVP.zip file is 4.38GB (compressed).  This is too big for Github to accept (32MB max) so I have put it out on Google Drive.  It took 2.2 hours to upload - be patient when downloading.

## MVP 1.0

https://drive.google.com/drive/folders/0B-63rlluTVV5dHBxQWROM29MNUk?usp=sharing

## MVP 1.2
https://drive.google.com/open?id=0B-63rlluTVV5YUFXb0NiQ2NUVm8

This is the same functionality as 1.0 with these changes:

- Reorganized into one directory.
- Uses smbus2 to give better accuracy for the temperature
- Persisted variables are stored in a python file (variables.py)

After creating the image and installing, the following steps need to be done:

- Set up wifi access for your network.
- from a terminal run:

> python /home/pi/MVP/python/testScript.py

> bash /home/pi/MVP/scripts/webcam.sh

> bash /home/pi/MVP/scripts/render.sh

There should be no errors.  This will produce data and a picture, and put them to the website.
