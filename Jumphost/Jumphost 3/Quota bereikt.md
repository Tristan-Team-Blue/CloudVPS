<h1> De klant geeft aan het quota bereikt te hebben </h1>

<h2> Controleren </h2>

 - [ ]  Controleer of je het Tenant ID hebt. (kan je vinden in de [BO](https://bo.infra.cloudvps.com/) onder het account, bij de "AuthUser" Projecten tabblad)
  - [ ]  Controleer of de klant bekend is.
  - [ ]  Controlleer of de klant zijn/haar facturen netjes betaald, mocht dit niet het geval zijn in overleg met Sales bespreken of de klant zijn/haar quota opgehoogd mag worden.
  - [ ]  Controlleer of de klant nogsteeds tegen zijn/haar quota aan zit, dit kan je bijvoorbeeld doen door op het Project in te loggen via de BackOffice. (het kan gebeuren dat de klant een test heeft gedaan waardoor hij de quota niet meer nodig heeft.)

**Let op dat het niet gaat om de network policy's zoals de neutron policy's. Deze komen zelden voor en worden niet verhoogd met het verdubbelen van de quota's. Volg hiervoor de onderstaande uitleg verhoge neutron policy's etc.**
`Als het gaat om een Openstack Legacy (Openstack 1) project dient er eerst vanuit de klant een geldige reden te komen waarom hij zijn/haar quota geupgrade wilt zien, raad hierbij ook Openstack 2 aan. Wanneer de klant een geldige reden heeft gestuurd dient er toestemming gevraagd te worden vanuit het Openstack Team.`
`Als het gaat om een testaccount worden deze alleen verhoogd zodra het project in production modus staat.`

<h2> Hoe verhoog je het quota? </h2>

Het quota kan je verhogen door het volgende commando uit te voeren:

```
ams reset-quota UUID --mode double
```