

Flan Scan is a lightweight network vulnerability scanner. With Flan Scan you can easily find open ports on your network, identify services and their version, and get a list of relevant CVEs affecting your network.

Flan Scan is a wrapper over Nmap and the vulners script which turns Nmap into a full-fledged network vulnerability scanner. Flan Scan makes it easy to deploy Nmap locally within a container, push results to the cloud, and deploy the scanner on Kubernetes.

Procedure of installation and using guide . 
1- simply install git clone https://github.com/cloudflare/flan flanscan (website:https://github.com/cloudflare/flan)
2- Cd flanscan
3- check ip of your target (nslookup  website)
4- make docker installed and check by command docker --versioin
5- nano ./shared/ips.txt  
6- write of ip that you have found above by nslookup)
7- confirm by this command  nano ./shared/ips.txt  
8- make by command make build
9- make  by command start scan
10- you write for specific target by this command 

sudo  nmap -sV -oX result -oN - -v1 $@ --script=vulners.nse -p _ ( _ mean port Number) website

Enclosed some snapshot during installation and result for your overlook. 

Its better you can use kali operating system in order to avoid package installation becuase kali perinstalled most of software by default.

CASE STUDY NO:1

Moreover, You can see below target if port is closed you will get this below result if open they you will get result as you can see snap shots are attached.  ref. snapshot Screenshot_2022-04-06_17_56_54.png

sudo  nmap -sV -oX result -oN - -v1 $@ --script=vulners.nse -p 80 icebreakerspro.com

# Nmap 7.92 scan initiated Wed Apr  6 17:24:44 2022 as: nmap -sV -oX resut -oN - -v1 --script=vulners.nse -p 80 icebreakerspro.com
Nmap scan report for icebreakerspro.com (34.134.15.26)
Host is up (0.0015s latency).
rDNS record for 34.134.15.26: 26.15.134.34.bc.googleusercontent.com

PORT   STATE    SERVICE VERSION
80/tcp filtered http

Read data files from: /usr/bin/../share/nmap
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Wed Apr  6 17:24:46 2022 -- 1 IP address (1 host up) scanned in 1.41 seconds
                                                                                           

Regards
Jamal hussain shah 




