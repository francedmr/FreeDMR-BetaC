 FreeDMR-Installer-Docker-Version
 --------------------------------

 This repo is to help you install a basic FreeDMR STAND ALONE Server and a HBMonv2 Dashboard to leaving a BASIC system to work with. 

 However, the **DOCKER** system that Simon Adlem, G7RZU <g7rzu@gb7fr.org.uk> is the **RECOMMENDED** way to install FreeDMR.
 
 See https://gitlab.hacknix.net/hacknix/FreeDMR/-/wikis/Installing-using-Docker-(recommended!) for more details.

 To install using the docker method from your server console enter the following command.


         apt-get update && apt upgrade
         curl https://github.com/francedmr/FreeDMR/-/raw/master/FreeDMR-Beta3/docker-compose_install.sh | bash	


 


 <hr>

FreeDMR-Installer-FRANCE-DMR-Version
--------------------------------

If you are not comfortable with DOCKER, you can set your server up using this script and answer some basic questions
There are a small number of repo's that may be downloaded which will not be configured by this script and need to be
compiled and/or setup if you wish to use them.

Depending on the install method you choose, you may need to provide some of the following details during the install
process.
 
1. NAME         - What you want to call the server
	
2. PORT         - Which you want the Hotspots or Repeaters to access your server
	
3. PASSWORD     - Used to authenticate Hotspots or Repeaters to access your server

4. IP ADDRESSES - This will depend on wether you are running just a FreeDMR Server or setting up a DASHBOARD remotely

The process of setting up your new server will take around 10 mins depending on you server speed and Internet speed.

You can run this script again if you want to reset back to the default STAND ALONE state at anytime. HOWEVER, BACKUP
your current config. If you don't, the settings will be lost for ever.


Install FreeDMR Server and/or HBMonv2 Dashboard
-----------------------------------------------

This will install and setup the FreeDMR Server With or With Out a Dashboard

To execute this script you have 2 option. The second option downloads the install script only and then executes it and
the first download the GIT on to your machine.

I recommend SUDO mode (Method 1).

Method 1

	cd /opt
	git clone https://github.com/francedmr/.FreeDMR-Beta3.git
	cd /opt/FreeDMR-Beta3
	bash install.sh
	

You can setup the dashboard to monitor the Server either locally or remotely.

or

Method 2

	wget https://github.com/francedmr/FreeDMR-Beta3/-/raw/main/install.sh -O install.sh && bash install.sh



