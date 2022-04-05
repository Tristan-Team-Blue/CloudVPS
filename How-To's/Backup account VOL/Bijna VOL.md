<h1> Backup account is FULL melding </h1>

Voorbeeld: [BACKUP Backupaccount vps49195 is full!](https://cerberus.office.xl-is.net/index.php/profiles/ticket/YHS-46535-822/conversation)

In het ticket, zul je een vpsnummer tegenkomen. Hiermee kan je het account opzoeken.

Je zult hiervoor de volgende commando's gebruiken:

```
backuptool stats vpsNUMMER
```

Hiermee zul je de volgende gegevens tegenkomen:

~~~
Backupserver..: backup-044.cloudvps.com
Username......: vps49195
Handle........: BGE00071
Quota.........: 200GB
Quota used....: 186GB (100%)
Quota avail...: 1.4GB
Inodes........: 52428800
Inodes used...: 761692 (2%)
Inodes free...: 51667108

Quota report for the last 7 days:
Date            Account                   Quota      Used       Free       %    
2022-04-05      vps49195                  200GB      186GB      1.4GB      100% 
~~~

Dan kijken we in dit geval naar het stukje == Quota used....: 186GB (100%) ==