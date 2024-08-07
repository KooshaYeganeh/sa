# sa

Scan with Common Security Tools with one Command on **openSUSE**

![SUSE](https://en.opensuse.org/images/f/f2/Button-laptop-colour.png)

## Tools

1 - **clamAV**  
2 - **RKHunter**  
3 - **LMD : Linux Malware Detect**  
4 - **chkrootkit**  
5 - **Lynis**

## Install

```
cd /tmp && wget https://github.com/KooshaYeganeh/sa/archive/refs/heads/main.zip && unzip main.zip && [ -d "/opt/script" ] && echo "Directory exists" || sudo mkdir /opt/script && cd sa-main && sudo mv sa /opt/script && echo "sa Installed [ OK ]" && cd && echo "Note : sa Tool is currently in /opt/script Directory"
```

Note : If you run the script for the first time, it will check whether the software is installed on your system or not. If the software is not installed, it will automatically install the software on your system.

Note : If you don't want to scan all devices with Ansible, you can install the RAM file on your system.

```
sudo rpm -ivh sa-1.0.0.noarch.rpm
```


## Use


Scan All : 

```
./sa -a or ./sa --all
```

Update Tools : 

```
./sa -u or ./sa --update
```

Scan All Hosts:

```
./sa --hosts
```


Help :

```
./sa -h or ./sa --help
```


