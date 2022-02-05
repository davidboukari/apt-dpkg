# apt-dpkg

```
apt-cache search package
apt-get install package

# List all installed package 
dpkg -l 

dpkg -l |grep fail2ban
ii  fail2ban                             0.11.1-1                              all          ban hosts that cause multiple authentication errors


# List all file of a package
dpkg -L fail2ban
/.
/etc
/etc/default
/etc/default/fail2ban
/etc/fail2ban
/etc/fail2ban/action.d
/etc/fail2ban/action.d/abuseipdb.conf
/etc/fail2ban/action.d/apf.conf
/etc/fail2ban/action.d/badips.conf
/etc/fail2ban/action.d/badips.py
...

```
