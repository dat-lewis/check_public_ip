check_public_ip
===============

Use
----

Check current IP and send changes to your email

Installation
----

Download the script and run the following command:

```
chmod +x check_public_ip
```
run "crontab -e" and add the following line

```
50 * * * * /script/directory/check_public_ip
```

Configuration
----

Change the following settings so it fits your needs

```
SNTTO="mail@domain.com"                     # recive address  
SBJCT="IP changed on host foo.domain.com"   # subject
PIP="/tmp/PIP"                              # temp dir
FRM="root@domain.com"                       # from header
```

Information
----

To use this script you need a working mail package installed on your server (e.g. sendmail, exim4, postfix,...)
