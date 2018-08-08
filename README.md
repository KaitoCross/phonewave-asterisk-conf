# phonewave-asterisk-conf
dongle.conf contains all configuration needed by chan_dongle. you will have to adjust it at certain points (for example putting the PhoneWaves mobile phone number in there)  
extension.conf contains the small dialplan that forwards the incoming call to the user 4001 if the user is logged in.  
modules.conf activates needed modules of asterisk  
sip.conf is the general configuration for the sip users which shall have access to this server. User 4001 is set up there and you just need to replace the password (secret=passwordhoeshere) with a strong one there  
copy these files into /etc/asterisk after having edited them and restart asterisk with sudo service asterisk restart. Have fun!
