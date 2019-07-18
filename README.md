# mac_changer
It is a simple tool which helps you to change your MAC address of your system.
It is a command line tool,requiring python2.7.
You need to provide interface and new MAC that needed to be changed.
ex root@kali:~#python mac_changer.py -i interface_name -m new_mac_address 
to know interface name type  ifconfig -a you can see a list of interfaces and their mac address(ether).
use --help for complete details.
