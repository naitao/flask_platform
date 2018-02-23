# flask_platform

# 1. To make sure you can use pip(python3.5) and pyscaffold with your EC2 instance (Ubuntu) smoothly, the following packages need to be pre-installed before the step 2-8:
#  $sudo apt-get update
#  $sudo apt-get install python3
#  $sudo apt-get install python3-pip
#  $sudo mv /usr/bin/python /usr/bin/python2; sudo ln -s /usr/bin/python3.5 /usr/bin/python
#  $sudo pip install pyscaffold
#  $pip install -U setuptools
# 2. The webapp server will be run on the EC2 instance. We assume that you have cloned flask_platform repo from GitHub when you are reading this file.
# 3. On EC2 instance(Ubuntu is recommended), before using flask_platfrom module, we need to pre-install flask module first (This module is offical python module)
#	$sudo pip install flask
# 4. Also, we need to install systeminfo module from GitHub (This is an informal module that was required in this assignment):
# $sudo pip install git+https://github.com/naitao/systeminfo.git
# 5. On EC2 instance, execute the system command which has been installed by flask_platform:
#	$comp30670_flasktest
# You will see that a web server is booting up and the current console was hold on.
# 6. On your local system (laptop or PC desktop), execute the following command on console or Terminal window:
# $ssh -i "peng1.pem" ubuntu@ec2-34-211-89-227.us-west-2.compute.amazonaws.com -N -L 5000:localhost:5000
# 7. Finally, open a browser and input url:
# http://localhost:5000
# Then, you will be able to see the system info displayed on you browser web page
# 8. You can also execute system command like below:
#    $/usr/local/bin/comp30670_flasktest
# And if you enabed port 5000 on EC2 instance opening to internect, you can just input your instance's public domain name with urlL
#    http://your~url:5000
