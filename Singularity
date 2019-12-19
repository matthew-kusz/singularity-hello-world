Bootstrap:docker  
From:ubuntu:18.04

%runscript
echo "This gets run when you run the image!"
exec /bin/bash /code/hi_there.sh "$@"

%post  
echo "This section happens once after bootstrap to build the image."
echo "You can use this section to install things."
mkdir -p /code
apt-get update -y
apt-get install -y vim
apt-get clean
echo 'echo 'Hi there'' >> /code/hi_there.sh
chmod u+x /code/hi_there.sh  
