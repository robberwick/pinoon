Pi Noon
=======

Mini Pi Noon code
-----------------

Ensure [pinoon](pinoon) init.d script file contains correct project install path, then setup the init.d script.

	sudo cp /home/pi/Projects/pinoon/pinoon /etc/init.d/  
	sudo chmod +x /etc/init.d/pinoon  
	sudo update-rc.d pinoon defaults  

Or for a simpler service install, just run with *sudo* permission the [install.sh](install.sh) file.

	sudo chmod +x *.sh  
	sudo ./install.sh  

### You must install bluetooth service and cwiid python module

	sudo apt-get install --no-install-recommends bluetooth  
	sudo apt-get install python-cwiid  

### Installing I2C, first enable it in raspi-config

	sudo apt-get install i2c-tools  
	sudo apt-get install python-smbus  
