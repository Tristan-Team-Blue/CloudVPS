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

Dan kijken we in dit geval naar het stukje 

> Quota used....: 186GB (100%)

Dit quota percentage tellen we op bij

> Inodes used...: 761692 (2%)

Als de 2 bij elkaar minimaal 100% is, dan zit het backupaccount echt vol.

Hierna kunnen we de klant gaan mailen. Hiervoor gebruik je het volgende Snippit:
~~~
Beste klant,

Graag willen wij uw aandacht vestigen op uw back-upaccount.

Momenteel heeft het account 100% van zijn quotum gebruikt, wat betekent dat het account vol is. Dit kan leiden tot ongewenste situaties.

Er zijn 3 oplossingen beschikbaar:

1. **Upgrade uw back-upaccount (als u een CloudVPS-back-upaccount gebruikt)**
Als u uw back-upaccount wilt upgraden, raadpleegt u de onderstaande URL voor onze prijspagina en stuur een e-mail naar support@cloudvps.nl met betrekking tot dit back-upaccount en in welke grootte het account moet worden geüpgraded:
(voor prijzen, zie de URL hieronder)
https://www.cloudvps.com/configurator/prices/

2. **Verlaag de retentie van de back-ups.**
Als u extra wekelijkse en/of maandelijkse retentie hebt gegeven, probeer deze dan te verlagen en verwijder de
week en/of maand van de back-upserver om de ruimte vrij te maken die niet meer nodig is.
De retentie kan worden verlaagd via het CloudVPS Backup Installer met behulp van de configuratie editor en de back-ups kunnen worden gewist met behulp van (S)FTP of via het installatieprogramma met behulp van de back-upverkenner, optie.

3. **Ruim onnodige bestanden op van de server en back-upserver.**
Controleer of er onnodige bestanden en/of mappen op de VPS staan die kunnen worden verwijderd. Als er zijn bestanden en/of mappen die geen back-up hoeven te maken, plaats ze op de uitsluitingslijst van rsync (kan worden gedaan via het installatieprogramma met behulp van de lijst Met uitsluitingen Optie. Zorg er ook voor dat u deze bestanden en/of mappen van de back-upserver verwijdert dit kan ook met behulp van (S)FTP of via het Installatieprogramma met behulp van de Backup Explorer optie.

Handleiding:
De CloudVPS Backup Operation Manual vindt u hieronder:
http://download.cloudvps.com/pub/files/scripts/backup/cloudvps-backup-manual.pdf

Ondersteuning:
Voordat u contact opneemt met CloudVPS, moet u ervoor zorgen dat u de opties 2 en 3 hebt bekeken en de handleiding gelezen hebben, anders kunnen we u niet volledig helpen en ondersteunen.
Als u niet weet wat het beste is om te doen, stuur dan een e-mail naar support@cloudvps.nl met betrekking tot dit back-upaccount en vermeld uw vraag
~~~

