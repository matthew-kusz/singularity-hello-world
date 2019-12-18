Bootstrap:docker  
From:ubuntu:18.04

%environment
GREET_BASE=/code
export GREET_BASE

%runscript
echo "This gets run when you run the image!" 

%post  
echo "This section happens once after bootstrap to build the image."
echo "You can use this section to install things."
mkdir -p /code
apt-get update -y
apt-get install -y vim  
echo "Hi there" >> /code/hi_there.sh
chmod u+x /code/hi_there.sh  
