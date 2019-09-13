Test Cases en Test Matrix
===

Om te valideren dat je applicatie voldoet aan de requirements moet je testen. Dat kan op een aantal manieren. Hier beschrijven we de zogenaamde 'Funcationele Tests'. 

Door test cases te relateren aan use cases worden enerzijds voorbeelden gegeven van waar het systeem precies mee moet kunnen werken. Anderzijds beschrijft dit ook hoe het systeem
reageert wanneer de gegevens onjuist zijn (de uitzonderingen). Aangezien het gebruik van
het systeem al gemodelleerd is in de use cases, zullen test cases altijd aan use cases gekoppeld worden. Zie figuur 1 voor een voorbeeld.

<figure>
    <img src="{{site.url}}/{{site.baseurl}}/img/tests.png" alt="Figuur 1: Voorbeeld van een testplan.">
    <figcaption>Figuur 1: Voorbeeld van een testplan</figcaption>
</figure>

Bij het voorbeeld is dit niet het geval, maar het is prima mogelijk om in een testplan een volgorde aan te brengen. Een voorbeeld hiervan is het testen van het registreren en inloggen van gebruikers. Als eerste kan een account aangemaakt worden, waarbij het registreren getest wordt. Deze aangemaakte account wordt vervolgens gebruikt om het inloggen mee te testen. Op deze manier zijn test cases eenvoudiger uit te voeren omdat er geen afhankelijkheid van bestaande data is. Zorg er wel voor dat in het testplan duidelijk is dat bepaalde cases elkaar dienen op te volgen.

###Testmatrix

Na het opstellen van de test cases is het mogelijk om een terugkoppeling te maken naar de
requirements. Hiervoor kan een test matrix opgesteld worden, waarin per test case aangegeven
wordt welke (delen van een) requirement getest wordt. Twee problemen kunnen aan het licht
komen: er is een (deel van een) requirement die nog niet getest wordt, of er is een test case
waarvoor geen requirement is. In het eerste geval ontbreekt er iets in een UI schets of use case, aangezien er een requirement is waarvoor nog geen interac􀦞e beschreven is. In het laatste geval blijkt er uit het analyseproces een nieuwe requirement te zijn ontstaan; dit betekent dat de lijst met requirements uitgebreid zal moeten worden.

Figuur 2 toont de matrix die aansluit bij de voorbeelden die in dit document zijn opgevoerd. Wat hieruit duidelijk wordt is dat requirement FR-01 in zijn volledigheid nog niet getest wordt. Dit impliceert dat er nog geen test cases zijn opgesteld hiervoor. Maar, er is ook nog geen use case voor beschikbaar: dit zal dus eerst uitgewerkt moeten worden. Wanneer dit gedaan is, kunnen tests worden opgesteld en wordt de matrix bijgewerkt.

<figure>
    <img src="{{site.url}}/{{site.baseurl}}/img/matrix.png" alt="Figuur 2: Voorbeeld van een testmatrix.">
    <figcaption>Figuur 2: Voorbeeld van een testmatrix.</figcaption>
</figure>

Wat ook naar voren komt uit de tabel is dat beperking B-02.2 niet getest wordt. Deze beperking
kwam neer op het niet leeg mogen zijn van de omschrijving van een verkoop. In het testplan is echter geen case opgenomen die dit valideert. Hiervoor dient dus een testcase toegevoegd te
worden; in dit geval is er reeds een toepasselijke use case beschikbaar.

