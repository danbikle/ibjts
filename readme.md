readme.md

Login to your ubuntu box, ubuntu laptop, or ubuntu virtualbox.

If you have no git on your ubuntu, install it like this:

```
apt-get install gitk
```

After git install, do this:

```
cd ~
git clone https://github.com/danbikle/ibjts.git
```

Download IntelliJ:

https://www.jetbrains.com/idea/download/


I got this file:

```
~/Downloads/ideaIC-14.1.2.tar.gz
```

Maybe you will get something newer.

Install it. Demo:

```
tar zxf ~/Downloads/ideaIC-14.1.2.tar.gz
ln -s idea-IC-141.713.2 idea
```

Enhance your path:

```
echo 'export PATH=~/idea/bin:$PATH' >> ~/.bashrc
```

Start IntelliJ:

```
~/idea/bin/idea.sh
```

Activate: Import Project

You want this folder fed to Import-Project: ibjts

Click through Import-Project wizard accepting all defaults.

If all goes well you should have a new project.

It should have two modules.

The corresponding folders should be these:

```
ibjts/samples/
ibjts/source/
```

Next, find $10k Minimum (or IRA account) to open Interactive Brokers Account.

Then, get an account with Interactive Brokers:

http://www.google.com/search?q=How+to+open+Interactive+Brokers+Account

After you get the account, download their Trader Workstation (TWS) software.

For the IB-API, TWS is a server.

TWS can also act as a client which behaves like a spreadsheet.

As a client it allows you to enter orders and see prices.

http://www.google.com/search?q=Interactive+Brokers+what+is+Trader+Workstation
http://www.google.com/search?q=Interactive+Brokers+Download+Trader+Workstation

After I download TWS, I can start it with one line of code:

```
cd ~/IBJts/
java -cp jts.jar:total.2013.jar -Xmx512M -XX:MaxPermSize=256M jclient.LoginFrame . &
```

Once it is up I configure it to act as an API server:

http://www.google.com/search?q=Interactive+Brokers+TWS+enable+API+7496

After the API server is up I click this class in IntelliJ and ask it to run:

https://github.com/danbikle/ibjts/blob/master/samples/Java/apidemo/ApiDemo.java

If a Swing client appears and it allows me to connect to the TWS-API-server,
I am happy.

Holler if you have questions:

dan@bot4.us

(add not-spam to subject)

