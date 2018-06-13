# LinuxServerConfiguration #

This is a project for the Udacity [FSND Course](https://www.udacity.com/course/full-stack-web-developer-nanodegree--nd004).

## The IP Address of the Server for this project is 18.222.105.219 ##
## The SSH port is 2200 ##
## The complete URL to the hosted web application is http://westalabamabeecompany.com ##
## Software that has been installed: ##
  * Apache2
  * Postgresql
  * Flask
  * SqlAlchemy
## Configuration Changes Made ##
  * Port 2200 was set for SSH in the /etc/ssh/sshd_config file
      * Note that on AWS it is very imortant to do this AFTER that port has been opened on AWS!!
  * Remote login apart from SSH has been disabled.
  * The application is installed in the /var/www/FlaskApp/FlaskApp subdirectory
  * The file that contain the flask application logig is __init__.py
  * A virtual environment called WABCO was created
  * The /etc/apache2/sites-available/FlaskApp.conf file was edited to include westalabamabeecompany.com and information on the virtual environment
## A user called grader has been created ##
  * To SSH into the server with the grader user:
    * ssh grader@18.222.105.219 -i ~/.ssh/grader -p 2200
      * The passphrase is M@y$2118

## Credits
  * I was assisted with problems in installation and configuration by Vladyslav Z. from freelancer.com
