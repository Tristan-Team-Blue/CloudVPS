<h1> Dit kan pas zodra de backuptool werkt!!!!!!! </h1>

<h1> Critical error occurred during the backup </h1>

Voorbeeld: [Critical error occurred during the backup!](https://cerberus.office.xl-is.net/index.php/profiles/ticket/ACB-76466-976)

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

Kijk of de backupserver aangepast is:

> Backupserver..: backup-044.cloudvps.com

<h2> Vergeet niet het snippit aan te passen! </h2>

Hierna kunnen we de klant gaan mailen. Hiervoor gebruik je het volgende Snippit:
~~~
Beste klant,

Graag willen wij uw aandacht vestigen op uw back-upaccount.

Het backup account staat gelinked met de verkeerde backup server.
Graag willen wij u verzoeken om de backup server aan te passen.

Deze mag aangepast worden naar server backup-045.cloudvps.com.

De instellingen die in het script gebruikt zijn.
Backupserver...: backup-028.cloudvps.com


Mocht u nog meer vragen hebben, kunt u deze altijd stellen.

Heeft u naar aanleiding van dit bericht nog een vraag of opmerking? Stuurt u
deze dan naar de CloudVPS Servicedesk op support@cloudvps.com. Wij zullen u zo
spoedig mogelijk antwoorden.

#comment Vergeet niet de Backupservers aan te passen
~~~

