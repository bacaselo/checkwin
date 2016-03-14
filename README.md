# checkwin
checkwin is a Xymon script that retrieves data from a Windows machine.

This is a script that allows Xymon to pull data from a windows machine. Our network model only allows for connections outbound from our management network so I thought I would spend the time to write this script. For it to work you will need to get a copy of check_nt on your machine. This is the client that is used to speak to nsclient++ that is used in Nagios. When you install the Nagios package or port you should find this binary (eg its in the net-mgmt/nagios port on FreeBSD)
NSClient++ is available at https://nsclient.org/download/
This script was used against version 0.3.5.

IMPORTANT UPDATE - january 2012: - **this external Xymon perl script was adapted to work with the more powerfull check_nrpe Nagios binary.** 
This new script was used against NSClient++ version 0.3.9.
To get all test to work you need to paste the external plugins in the folder "C:/program files/NSClient++/scripts" of the target server that you want to monitor.
