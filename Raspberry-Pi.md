### Setting up your Raspberry Pi

Every time I get a new Raspberry Pi from my college's lab, I have to set it up. So, I decided to pen down the steps. Here are the steps you should follow if you want to set up your raspberry pi.

1.  Power up your pi. Connect the ethernet cable to your laptop.
2.  Find out the IP address of your pi.

arp -a

When you type this, something like this should come up.

(192.168.1.1) at 48:ee:0c:be:55:7c [ether] on eno1

This is the IP address.

(192.168.1.1)

2\. ssh into the pi.

ssh pi@ip_address_of_pi

3\. You will have to enter the password. The default password is :

raspberry

4\. Enable [VNC](https://en.wikipedia.org/wiki/Virtual_Network_Computing) in pi.

sudo raspi-config

Then go to advanced options and enable VNC.

5\. For VNC, I strongly suggest you use the Chrome extension for VNC. Download it from [here.](https://chrome.google.com/webstore/detail/vnc%C2%AE-viewer-for-google-ch/iabmpiboiopbgfabjmgeedhcmjenhbla?hl=en)

Launch the VNC. Type in your credentials and enter the IP address that you got in step 1.

default username : pi\
default password : raspberry

You should now see the desktop of raspberry pi on the VNC !
