# flask_platform

# 0. The webapp server will be run on the EC2 instance. We assume that you have cloned flask_platform repo from GitHub when you are reading this file.
# 1. On EC2 instance(Ubuntu is recommended), before using flask_platfrom module, we need to pre-install flask module first (This module is offical python module)
#	$sudo pip install flask
# 2. Also, we need to install systeminfo module from GitHub (This is an informal module that was required in this assignment):
# $sudo pip install git+https://github.com/naitao/systeminfo.git
# 3. On EC2 instance, execute the system command which has been installed by flask_platform:
#	$comp30670_flasktest
# You will see that a web server is booting up and the current console was hold on.
# 4. On your local system (laptop or PC desktop), execute the following command on console or Terminal window:
# $ssh -i "peng1.pem" ubuntu@ec2-34-211-89-227.us-west-2.compute.amazonaws.com -N -L 5000:localhost:5000
# 5. Finally, open a browser and input url:
# http://localhost:5000
# Then, you will be able to see the system info displayed on you browser web page
