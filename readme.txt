ibjts/readme.txt

Login to your ubuntu box or laptop.

If you have no git on your ubuntu, install it like this:

apt-get install gitk

After git install, do this:

cd ~
git clone https://github.com/danbikle/ibjts.git

Download IntelliJ:

https://www.jetbrains.com/idea/download/

I got this file:
~/Downloads/ideaIC-14.1.2.tar.gz
Maybe you will get something newer.

Install it. Demo:

tar zxf ~/Downloads/ideaIC-14.1.2.tar.gz

ln -s idea-IC-141.713.2 idea

Enhance your path:

echo 'export PATH=~/idea/bin:$PATH' >> ~/.bashrc

Start IntelliJ:

~/idea/bin/idea.sh

Activate: Import Project

You want this folder fed to Import-Project: ibjts

Click through Import-Project wizard accepting all defaults.

If all goes well you should have a new project.

It should have two modules.

The corresponding folders should be these:

ibjts/samples/
ibjts/source/

