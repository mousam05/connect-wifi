# connect-wifi
dmenu based application for Linux that connects to the strongest open wireless network

##How to use:

###Packages required:
 The following packages must be installed on your system:
* dhcpcd (already installed by default on most linux distros)
* dmenu (from dmenu.suckless.org)

###Instructions:
1. copy wifi as /bin/wifi
2. copy dmenu_wifi as /bin/dmenu_wifi
3. replace wlp4s0 by the name of your wireless interface (for example, wlan0)
3. grant execute permission to above files by  
<pre>chmod +x /bin/wifi /bin/dmenu_wifi</pre>
4. modify sudoers file to allow execution of 'sudo dmenu_wifi' without password
5. bind the command 'sudo dmenu_wifi' to any key combination of your choice - there is an easy way to do this on most linux distros

Now the specified key combination will trigger a menu showing all wireless networks, strongest first. You can connect to any one of them!
