# apt-dpkg

## apt-mark
* Set at manualy or automatic installed package

## Update kernel
```
apt-cache policy linux-image-generic
linux-image-generic:
  Installé : 5.4.0.117.120
  Candidat : 5.4.0.117.120
 Table de version :
 *** 5.4.0.117.120 500
        500 http://fr.archive.ubuntu.com/ubuntu focal-updates/main amd64 Packages
        500 http://fr.archive.ubuntu.com/ubuntu focal-security/main amd64 Packages
        100 /var/lib/dpkg/status
     5.4.0.26.32 500
        500 http://fr.archive.ubuntu.com/ubuntu focal/main amd64 Packages
```




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

# apt-key
```
 apt-key list
/etc/apt/trusted.gpg
--------------------
pub   rsa4096 2020-05-07 [SC]
      E8A0 32E0 94D8 EB4E A189  D270 DA41 8C88 A321 9F7B
uid           [ unknown] HashiCorp Security (HashiCorp Package Signing) <security+packaging@hashicorp.com>
sub   rsa4096 2020-05-07 [E]

/etc/apt/trusted.gpg.d/ubuntu-keyring-2012-archive.gpg
------------------------------------------------------
pub   rsa4096 2012-05-11 [SC]
      790B C727 7767 219C 42C8  6F93 3B4F E6AC C0B2 1F32
uid           [ unknown] Ubuntu Archive Automatic Signing Key (2012) <ftpmaster@ubuntu.com>

/etc/apt/trusted.gpg.d/ubuntu-keyring-2012-cdimage.gpg
------------------------------------------------------
pub   rsa4096 2012-05-11 [SC]
      8439 38DF 228D 22F7 B374  2BC0 D94A A3F0 EFE2 1092
uid           [ unknown] Ubuntu CD Image Automatic Signing Key (2012) <cdimage@ubuntu.com>

/etc/apt/trusted.gpg.d/ubuntu-keyring-2018-archive.gpg
------------------------------------------------------
pub   rsa4096 2018-09-17 [SC]
      F6EC B376 2474 EDA9 D21B  7022 8719 20D1 991B C93C
uid           [ unknown] Ubuntu Archive Automatic Signing Key (2018) <ftpmaster@ubuntu.com>

```
