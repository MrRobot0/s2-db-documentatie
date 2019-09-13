Use Cases
=========

Op basis van een UI-schets schetsen zijn use cases op te stellen die precies aangeven hoe de interactie met het systeem plaatsvindt. Alhoewel er geen exacte richtlijn te geven is, zijn handelingen die neerkomen op het wisselen van schermen of pagina’s typisch geen eigen use case maar stappen hierbinnen. Een use case wordt gebruikt om handelingen die de toestand (gegevens) van het systeem gebruiken of beïnvloeden te documenteren.

In de tabel hieronder is een voorbeeld te zien van een uitgewerkte use case, overeenkomstig met een van de eerder getoonde [UI schets](UI-Schetsen). De use case beschrijft hoe de functionele [requirement](Requirements) precies vervuld kan worden. Er wordt vanuit gegaan dat er standaard geen problemen optreden bij het uitvoeren van de use case; dit wordt ook wel de “happy flow” genoemd. 

Mocht er bij bepaalde stappen een probleem op kunnen treden, dan wordt hier een uitzondering genummerd bij aangemerkt. In dit voorbeeld is per uitzondering aangegeven welke beperking ondervangen wordt; ook de use case zelf is voorzien van een identificatie.

###Requirements

    FR-01 De gebruiker moet een overzicht van alle verkopen kunnen inzien.
        B-01.1 Overzichten van verkopen zijn op maanden, kwartalen of jaren.
        K-01.1 Overzichten dienen oplopend en aflopend gesorteerd te kunnen worden.
    FR-02 Er kunnen nieuwe verkopen toegevoegd worden aan het systeem.
        B-02.1 Voor verkopen wordt een omschrijving, het bedrag en het tijdstip vastgelegd.
        B-02.2 De omschrijving van een verkoop mag niet leeg zijn.
        B-02.3 Alleen leidinggevenden mogen de datum van een verkoop aanpassen; 
        anders is deze altijd het moment van invoeren.
        FR-03 Het is mogelijk om geld terug te geven aan klanten (voor het ruilen van artikelen).

###Use-case beschrijving

|*Naam*|UC01: Nieuwe verkoop toevoegen|
|----|------------------------|
|*Samenvatting*|Na het ingeven van de vereiste gegevens wordt dit als verkoop aan het systeem toegevoegd.|
|*Actors*|Verkoper, Leidinggevende|
|*Aannamen*|Geen|
|*Scenario*|<ol><li>De actor geeft aan een nieuwe verkoop te willen toevoegen</li><li>Het systeem toont een pagina waarop de gegevens ingevuld kunnen worden (zie B-02.1).</li><li>De actor voert zijn gebruikersidentificatie en de gevraagde gegevens in en bevestigt.</li><li>Het systeem controleert de ingevoerde gegevens en voegt de verkoop toe. [1][2]</li></ol>|
|*Uitzonderingen*|<ol><li>Niet alle benodigde gegevens zijn ingevuld. Toon een melding en ga terug naar stap 3. (B-02.2)</li><li>De verkoopdatum is aangepast en de actor is geen leidinggevende. Zet de datum op de huidige datum en tijd en ga verder met de use case. (B-02.3)</li></ol>|
|*Resultaat*|Er is een nieuwe verkoop toegevoegd aan het systeem.|

###Use-case diagrammen

Als je meerdere use-cases hebt, kan het zinvol zijn deze in een diagram weer te geven (zie Figuur 1). Hiermee kan goed worden getoond welke use-cases bij welke actoren horen. De waarde van zo'n diagram is beperkt, maar kan in sommige gevallen een aardig overzicht geven. Het is in geen geval een vervanging van de Use-Case Beschrijvingen. 

<figure>
    <img src="{{site.url}}/{{site.baseurl}}/Use Case Diagram.png" alt="Figuur 1: Voorbeeld van een Use Case diagram">
    <figcaption>Figuur 1: Voorbeeld van een Use Case diagram</figcaption>
</figure>

In het diagram zie je drie actoren (twee rollen en een extern systeem) en een viertal use-cases. In principe wordt er geen volgordelijkheid aangegeven in een use-case diagram.

###Bronnen
Om meer over use-cases te weten te komen kun je de volgende bronnen raadplegen:

* De oefening [Use Cases opstellen in Canvas](https://fhict.instructure.com/courses/8648/assignments/129651)
* De oefening [Use Case Diagrammen in Canvas](https://fhict.instructure.com/courses/8648/assignments/129650)
* [Alistair Cockburn's 'Writing Effective Use Cases'](https://www.bol.com/nl/p/writing-effective-use-cases/1001004001047678/) is het beste boek over use-cases. 
* Deze [presentatie van de Seidenberg School of CSIS](http://csis.pace.edu/~marchese/CS389/L9/Use%20Case%20Diagrams.pdf) geeft ook een aardig overzicht. 

