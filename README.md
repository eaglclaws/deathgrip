DEATHGRIP
=========================
-------------------------


What is Deathgrip
-------------------------

Deathgrip is a Python-based program which is used to encrypt and decript plain text messages by converting letters to numbers and using a mathmatical algorithm based on the time, date, and random integers. 

 Basic Usage
-------------------------

Deathgrip is ran in either encoder (-e) or decoder (-d) mode. You must specify an input file. You can optionally specify an output file. To encode "foo.txt" you could use:

    deathgrip -e -i foo.txt

As it would by default send that output to "output.txt", you would decode the output with:

    deathgrip -e -i output.txt -o bar.txt

Since we specified an output file for the decoder, the decoded message can be seen by opening "bar.txt"
    
A complete list of command line arguments can be seen with 

	deathgrip --help
    

Instalation
--------------------------

The recommended debian based instalation method is as follows:

    sudo $SHELL
    cd /tmp/
    git clone https://github.com/super-nathan/deathgrip.git
    cd /tmp/deathgrip
    dpkg-buildpackage -us -uc
    cd ../
    dpkg -i deathgrip_*_all.deb
    exit
    
All other Linux users should
	
	sudo $SHELL
    cd /tmp/
    git clone https://github.com/super-nathan/deathgrip.git
    cd /tmp/deathgrip
    cp deathgrip /usr/bin/
    cp deathgrip.conf /etc/
    exit

Authors
------------------------

Joseph Ko and Nathan Weber
