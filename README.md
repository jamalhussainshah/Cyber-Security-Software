# Cyber-Security-Software
Software installation 




RITA EASY INSTALLATION GUIDANCE. 

open website: https://github.com/activecm/rita

you will copy and past on terminal
wget https://github.com/activecm/rita.git


FORMATION OF .SH FILE

Create install.sh file by simply open text editor and past as given details with save as install.sh file any where
you like to store like in document or desktop. 

#!/bin/sh
echo "what is your name?"
read name
echo "How do you do $ name?"
read remark
echo "I am $ remark too!"


Now you have created install.sh file and ready for install rita.

now open terminal centos 7 and 

suppositely you will stored install.sh desktop then you will come to Desktop in terminal centos 7

jamal@>cd Desktop 
jamal@Desktop>



Download rita from attached rita file but unzip the file in order to you know location of rita folder in your system.

suppositely, you will stored in desktop then you will come to folder in (Desktop>rita-master) interminal 

jamal@Desktop>
jamal@Desktop>rita-master>



jamal@Desktop>rita-master>sudo chmod +x ./install.sh 
jamal@Desktop>rita-master>sudo ./install.sh


NOTE: During process of installation three question ask by system than you will click three times YES(Y) in order to 
compelete installation whole rita,zeek annd Monogo.

If you will required to install only rita without zeek and mongo then you will write below command.

jamal@Desktop>rita-master>sudo ./install.sh --disable-zeek --disable-mongo 

