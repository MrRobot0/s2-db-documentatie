Requirements
=========

Een functionele requirement beschrijft de handelingen die verricht kunnen worden met de applicatie. Iedere functionele requirement kan kwaliteitseisen en beperkingen bevatten die een
afbakening geven. 

### Verzamelen van requirements
Je kunt de eisen aan je systeem op meedere manier verzamelen:

* Interviews met stakeholders, zoals opdrachtgever en eindgebruiker;
* Bestuderen van documentatie, project-beschrijving en technische handleidingen;
* *Reverse Engineering* van een systeem dat lijkt hetgene dat je moet gaan maken;
* Door middel van *Prototyping* en de feedback die je daarop krijgt;
* Een focusgroep.

### Documenteren van requirements
Nadat je de eisen hebt geïnventariseerd kun je ze gaan documenteren. In eerste instantie kun je ze grofmazig opschrijven. We gebruiken in de volgende voorbeelden een simple verkoopsysteem. 

Dit is een voorbeeld van een requirement vastgelegd als User Story:

    Als Leidinggevende wil ik een overzicht van alle verkopen kunnen inzien 
    om een beeld te krijgen van hoe het gaat met het bedrijf.
    Als Leidinggevende wil ik een overzicht van de verkopen kunnen inzien per jaar om te kunnen vergelijken hoe de jaarlijke omzet er voor staat.
    Als Leidinggevende wil ik een overzicht van de verkopen kunnen inzien per kwartaal om te kunnen vergelijken hoe de kwartaalomzet er voor staat.
    etc..

Je ziet dat hier meteen verschillende variaties van de requirements als losse eis zijn opgenomen. Dat is handig om te doen als je later gaat prioriteren (zie onder). Het kan zomaar zijn dat niet alle overzichten even belangrijk zijn.

Een alternatieve manier om requirements op te schrijven zie je hier:

    FR-01 De gebruiker moet een overzicht van alle verkopen kunnen inzien.
        B-01.1 Overzichten van verkopen zijn op maanden, kwartalen of jaren.
        K-01.1 Overzichten dienen oplopend en aflopend gesorteerd te kunnen worden.
    FR-02 Er kunnen nieuwe verkopen toegevoegd worden aan het systeem.
        B-02.1 Voor verkopen wordt een omschrijving, het bedrag en het tijdstip vastgelegd.
        B-02.2 De omschrijving van een verkoop mag niet leeg zijn.
        B-02.3 Alleen leidinggevenden mogen de datum van een verkoop aanpassen; 
               anders is deze alijd het moment van invoeren.
    FR-03 Het is mogelijk om geld terug te geven aan klanten (voor het ruilen van artikelen).
        B-03.1 Alleen leidinggevenden zijn in staat om geld terug te geven aan klanten.
    K-ALG.01 Bij onjuiste invoer moet een duidelijke foutmelding getoond worden.

### Prioriteren van requirements

Wat niet getoond is in dit overzicht, is de prioritering van de requirements. Niet alles is even belangrijk en omdat er altijd sprake is van deadlines en beperkte budgetten moeten keuzes worden gemaakt. Om de meest relevante requirements op te kunnen leveren en dus ook je planning op orde te hebben, wordt iedere requirement voorzien van een prioriteit. Hoe de prioriteit uiteindelijk tot stand komt maakt niets uit; er wordt hoe dan ook begonnen met het uitwerken, ontwerpen en bouwen van de meest belangrijke feature.

1. MoSCoW

Een eenvoudige methode om te prioriteren is de MoSCow-techniek: Must (dit moet er zeker in), Should (zit zou er toch eigenlijk wel in moeten zitten), Could (dit is een optie) of Won’t (dit gaan we zeker niet doen).

Welke functionaliteit aan welke requirement wordt gekoppeld is iets wat in overleg met de opdrachtgever bepaald wordt. Per iteratie of oplevering kan deze prioritering herzien worden.
Het getoonde overzicht is al aardig uitgewerkt, maar het is prima mogelijk dat de eerste versie
van de requirements beknopter of simpeler zijn. 

2. Priority Poker

Een andere manier om te prioriteren, die goed werkt in een multi-disciplinair team is gebruik te maken van poker-kaarten. Elk lid van het team geeft voor zichzelf een bepaalde feature een priorteit. Tegelijkertijd draait iedereen zijn kaart om, waarna er (waarschijnlijk) discussie komt over de verschillen. Het doel is om consensus te bereiken.

3. 100 Dollar

Een derde techniek om te prioriteren is de 100-dollar methode. Elke requirement krijgt een geldbedrag toegewezen, maar er is een strikt budget van 100 dollar beschikbaar. Dit dwingt de stakeholders om kritisch te kijken naar wat ze echt belangrijk vinden. 

