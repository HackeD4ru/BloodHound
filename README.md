# BloodHound
Limitations

BloodHound.py currently has the following limitations:

Supports most, but not all BloodHound (SharpHound) features. Currently GPO local groups are not supported, all other collection methods are implemented.

Installation and usage

You can install the ingestor via pip with pip install bloodhound, or by cloning this repository and running pip install . from the project directory. BloodHound.py requires impacket, ldap3 and dnspython to function.

The installation will add a command line tool bloodhound-python to your PATH.

To use the ingestor, at a minimum you will need credentials of the domain you're logging in to. You will need to specify the -u option with a username of this domain (or username@domain for a user in a trusted domain). If you have your DNS set up properly and the AD domain is in your DNS search list, then BloodHound.py will automatically detect the domain for you. If not, you have to specify it manually with the -d option.
