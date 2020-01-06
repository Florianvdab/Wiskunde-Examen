# Wiskunde - Examen 07-01

## Hoofdstuk 6

### Cosinus Similariteit

![image-20200104155051206](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200104155051206.png)

𝑥⃗=(**3**,<u>2</u>,0,5,0,0,0,2,0,0) 

𝑦⃗=(**1**,<u>0</u>,0,0,0,0,0,1,0,2)

𝑥⃗∙𝑦⃗=**3∗1**+<u>2∗0</u>+0∗0+5∗0+0∗0+0∗0+0∗0+2∗1+0∗0+0∗2= 5 

‖𝑥⃗‖=√3∗3+2∗2+0∗0+5∗5+0∗0+0∗0+0∗0+2∗2+0∗0+0∗0= 6,48 

‖𝑦⃗‖=√1∗1+0∗0+0∗0+0∗0+0∗0+0∗0+0∗0+1∗1+0∗0+2∗2=2,24 

cos(𝑥⃗,𝑦⃗)= 0,31



### Correlatie

https://www.youtube.com/watch?v=sEN3FxQ5htg

**TI-84 Plus:**

**STAT - EDIT - Lijst invullen - Mode - Stat Diag = ON - STAT - CALC - LinReg = r**

(Niet gekend)

### Euclidisch

![image-20200104164042436](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200104164042436.png)

𝑥⃗=(0,−1,0,1)

𝑦⃗=(1,0,−1,0)

**√(0-1)² + (-1-0)² + (0+1)² + (1-0)² = 2**

### Jaccard

![image-20200104182409822](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200104182409822.png)

1,1,0,1,0,1

1,1,1,0,0,1

F00:1

F10:1

F01:1

F11:3

**3/(1+1+3) = 0.6**

### Edit-afstand

a) edit-afstand tussen abcdef en bdaefc 

delete ‘a’ → bcdef 

delete ‘c’ → bdef 

insert ‘c’ → bdefc 

insert ‘a’ → bdaefc

**4 bewerkingen nodig = edit distance ‘4’**

Of 

De aanwezig LCS is van lengte 4. 

length(abcdef) = 6 

length(bdaefc) = 6 

**6+6−2.4=4**



b) edit-afstand tussen abccdabc en acbdcab 

delete ‘c’ → abccdab 

delete ‘cc’ → abdab 

insert ‘c’ → acbdab 

insert ‘c’ → acbdcab 

**4 bewerkingen nodig = edit distance ‘4’**

of 

De aanwezige LCS is van lengte 5.
length(abccdabc) = 8 

length(acbdcab) = 7 

8+7−2.5=5

**In dit geval komt de ‘theoretische’ edit-afstand niet overeen met de werkelijke edit-afstand. De reden hiervoor is dat wij ‘cc’ in één keer kunnen verwijderen, maar dat de theoretische edit-afstand dit als 1 karakter zal behandelen en dus 2 operaties nodig heeft.**

### Hamming-afstand

Hamming-afstand = aantal bits die verschillen van elkaar
**d(000000, 110011)=4** 

**d(110011, 010101)=3** 

**d(010101, 011100)=2**

## Hoofdstuk 7.1

**Classificeren is het leren van een doelfunctie 𝑓 die elke verzameling attributen 𝑥⃗ afbeeldt op een vooraf gedefinieerd class label 𝑦.**

### Entropie

![image-20200105113005103](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105113005103.png)



### Gini

![image-20200105113024799](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105113024799.png)



### Classificatiefout

![image-20200105113054732](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105113054732.png)



### Informatiewinst

![image-20200105113226043](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105113226043.png)

### Oefeningen

#### Gini & Informatiewinst

![image-20200105114117563](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105114117563.png)



**Bereken de Gini-index voor de volledige verzameling aan training records.**

Kijken naar de Class, optellen, 
**C0 = 10 van de 20**
**C1 = 10 van de 20**

![image-20200105114459475](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105114459475.png)

![image-20200105114516314](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105114516314.png)

**Bereken de Gini-index voor het Customer ID en het Gender attribuut.**

Gini(customer ID) = 1 - 1 = 0 (geen informatie want elk record is gewoon een ID)

Eerst de C0(gender=female), C1(gender=female)

![image-20200105115133708](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105115133708.png)

![image-20200105115159255](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105115159255.png)

**Bereken de Gini-index voor het Car Type en Shirt Size attribuut gebruik makend van meervoudige splitsing.**

Meervoudig = kijken naar het totaal aantal van het car type. (Wel nog altijd C0 & 1 apart houden)

Family = 4

Luxury = 8

Sports = 8

![image-20200105115639137](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105115639137.png)

![image-20200105120706133](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105120706133.png)

![image-20200105121350854](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105121350854.png)



**Welk van de attributen verkies je?**

Car type heeft de laagste Gini-index, dus dit attribuut krijgt de voorkeur. Het geeft ook de hoogste informatiewinst. We kunnen dit ook m.b.v. de informatiewinst (Δ=Gini(dataset)−Gini(attribuut)) weergeven.
Voor Gender: Δ𝐺𝑒𝑛𝑑𝑒𝑟=1/2−0,48=0,02 

Voor Car type: Δ𝑐𝑎𝑟 𝑡𝑦𝑝𝑒=1/2−0,163=0,327 

Voor shirt size: Δ𝑠ℎ𝑖𝑟𝑡 𝑠𝑖𝑧𝑒=1/2−0,492=0,008 

Customer ID laten we hier achterwege, omdat het onmogelijk is om een beslissingsboom te maken waarbij voor elk record een afzonderlijke tak gemaakt wordt.

#### Entropie

![image-20200105134005872](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105134005872.png)

**Wat is de entropie van de verzameling aan training records?**



![image-20200105134647440](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105134647440.png)



**Wat is de informatiewinst van 𝑎1 en 𝑎2 in relatie tot de training records?**

![image-20200105134904866](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105134904866.png)

![image-20200105135009729](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105135009729.png)

**Voor 𝑎3, een continu attribuut, bereken de informatiewinst voor elke mogelijke splitsing.**

![image-20200105144257750](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105144257750.png)

![image-20200105144307520](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105144307520.png)

**Wat is de beste splitsing (tussen 𝑎1,𝑎2 en 𝑎3) rekening houdend met de informatiewinst?**

Volgens de informatiewinst is 𝑎1 de beste splitsing omwille van de hogere informatiewinst.

**Wat is de beste splitsing (tussen 𝑎1 en 𝑎2) rekening houdend met de classificatiefout?**

![image-20200105144335385](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105144335385.png)



**Wat is de beste splitsing (tussen 𝑎1 en 𝑎2) rekening houdend met de Gini-index?**

Gini(𝑎1)=0,344;Gini(𝑎2)=0,4938 ook hier krijgt 𝑎1 de voorkeur.

#### Classificatiefout

(Staat in principe niet op het formularium dus moet niet gekend zijn)

![image-20200105145045127](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105145045127.png)

**Bouw een beslissingsboom op basis van deze data, maak hiervoor gebruik van de classificatiefout als informatiewinstcriterium.**

Wij starten met de classificatiefout te bepalen van “habitable” 

![image-20200105145118026](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105145118026.png)

Vervolgens de classificatiefout en informatiewinst voor elk van de twee attributen

![image-20200105145142576](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105145142576.png)

![image-20200105145208601](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105145208601.png)

## Hoofdstuk 7.2

### Bayes Posterio Kans

![image-20200105162751936](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105162751936.png)



### Naïf Bayes Classificeren

![image-20200105162803947](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105162803947.png)

### Oefeningen

![image-20200105163612422](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105163612422.png)

**Schat de voorwaardelijke kansen voor P(A|+), P(B|+), P(C|+), P(A|-), P(B|-) en P(C|-).**

De voorwaardelijke kansen 

P(A=1|-) = 2/5 = 0,4 

P(B=1|-) = 2/5 = 0,4 

P(C=1|-) = 5/5 = 1 

P(A=0|-) = 3/5 = 0,6 

P(B=0|-) = 3/5 = 0,6 

P(C=0|-) = 0/5 = 0 

P(A=1|+) = 3/5 = 0,6 

P(B=1|+) = 1/5 = 0,2 

P(C=1|+) = 4/5 = 0,8 

P(A=0|+) = 2/5 = 0,4 

P(B=0|+) = 4/5 = 0,8 

P(C=0|+) = 1/5 = 0,2

**Maak gebruik van de geschatte voorwaardelijke kansen in de vorige vraag om het class label toe te kennen voor het testrecord (A=0, B=1, C=0) gebruik makend van naïve Bayes classificeren.**

![image-20200105165220550](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105165220550.png)





![image-20200105165231931](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105165231931.png)







**Schat de voorwaardelijke kansen met de m-schattingsmethode (p=1/2 en m=4)**

![image-20200105165613545](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105165613545.png)

P(A=0|+) = (2+2)/(5+4) = 4/9 

P(B=0|+) = (4+2)/(5+4) = 6/9 

P(C=0|+) = (1+2)/(5+4) = 3/9 

P(A=0|-) = (3+2)/(5+4) = 5/9 

P(B=0|-) = (3+2)/(5+4) = 5/9 

P(C=0|-) = (0+2)/(5+4) = 2/9 

P(A=1|+) = (3+2)/(5+4) = 5/9 

P(B=1|+) = (1+2)/(5+4) = 3/9 

P(C=1|+) = (4+2)/(5+4) = 6/9 

P(A=1|-) = (2+2)/(5+4) = 4/9 

P(B=1|-) = (2+2)/(5+4) = 4/9 

P(C=1|-) = (5+2)/(5+4) = 7/9

**Herhaal (b) gebruik makend van de voorwaardelijke kansen uit (c).**

![image-20200105165946936](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105165946936.png)

**Vergelijk de twee schattingsmethodes. Welke is beter? Waarom?**

Bij het vergelijken van de 2 methodes is de m-schatting een betere methode, omwille van het klein aantal trainingsrecords.



![image-20200105170526046](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105170526046.png)

**Schat de voorwaardelijke kansen voor P(A=1|+), P(B=1|+), P(C=1|+), P(A=1|-), P(B=1|-) en P(C=1|-) met dezelfde methode als in oefening 1.**

P(A=1|+) = 3/5 = 0,6 

P(B=1|+) = 2/5 = 0,4 

P(C=1|+) = 4/5 = 0,8 

P(A=1|-) = 2/5 = 0,4 

P(B=1|-) = 2/5 = 0,4 

P(C=1|-) = 1/5 = 0,2

**Gebruik de voorwaardelijke kansen uit (a) om het class label te voorspellen voor een testrecord (A=1, B=1, C=1) met naïve Bayes classificeren.**

![image-20200105170649437](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105170649437.png)

**Vergelijk P(A=1), P(B=1) en P(A=1,B=1). Is er een relatie tussen A en B?**

P(A=1) = 0,5
P(B=1) = 0,4
P(A=1,B=1) = 0,2
→ P(A=1,B=1)= P(A=1).P(B=1)
→ A=1 en B=1 zijn onafhankelijk.

**Herhaal de analyse uit (c) met P(A=1), P(B=0) en P(A=1,B=0).**

P(A=1) = 0,5
P(B=0) = 0,6
P(A=1,B=0) = 0,3
→ P(A=1,B=0)= P(A=1).P(B=0)
→ A=1 en B=0 zijn onafhankelijk.

**Vergelijk P(A=1,B=1|Class=+) met P(A=1|Class=+) en P(B=1|Class=+).**

P(A=1,B=1|Class=+) = 0,1
P(A=1|Class=+) = 0,3
P(B=1|Class=+) = 0,2
Omdat P(A=1|+).P(B=1|+) niet hetzelfde is als P(A=1,B=1|+) zijn A=1 en B=1 niet voorwaardelijk onafhankelijk (als gegeven is dat ze tot class + behoren)
Omdat ze niet voorwaardelijk onafhankelijk zijn, mogen we eigenlijk naïve Bayes niet toepassen op deze dataset.

## Hoofdstuk 7.3

#### Prediction & Target

![image-20200105171712159](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105171712159.png)

Confusion matrix en misclassificatieratio (aantal verkeerd geclassificeerde t.o.v. totaal aantal geclassificeerde records).

Precision, recall en f1-maat.

![image-20200105171738634](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105171738634.png)

De misclassificatieratio bedraagt dan:

![image-20200105171757257](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105171757257.png)

![image-20200105171808607](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105171808607.png)

## Hoofdstuk 8

### Oefening

Maak gebruik van het k-means algoritme en de Euclidische afstandsmetriek om de volgende 8 voorbeelden te groeperen in 3 clusters: A1=(2,10), A2=(2,5), A3=(8,4), A4=(5,8), A5=(7,5), A6=(6,4), A7=(1,2), A8=(4,9). De op de Euclidische afstand gebaseerde afstandsmatrix is hieronder gegeven:

![image-20200105172148351](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105172148351.png)

Veronderstel dat de initiële centroïdes A1, A4 en A7 zijn. Voer het k-means algoritme één maal uit. Toon op het einde van deze ronde:

**de nieuwe clusters**

seed1 = A1 = (2,10) 

seed2 = A4 = (5,8) 

seed3 = A7 = (1,2)

![image-20200105172344440](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105172344440.png)

![image-20200105172354229](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105172354229.png)



**de centra van de nieuwe clusters**

De centra van de nieuwe clusters zijn: C1 = (2; 10) 

C2 = ((8+5+7+6+4)/5; (4+8+5+4+9)/5) = (6; 6) 

C3 = ((2+1)/2; (5+2)/2) = (1,5; 3,5)

**teken een rechthoekig assenstelsel met alle 8 punten en duid de clusters aan met hun centra** 

![image-20200105172432103](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105172432103.png)



**hoeveel iteraties extra zijn nodig voor er convergentie optreedt?**

![image-20200105172445452](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200105172445452.png)

## Hoofdstuk 1

**<u>Oefening 1</u>**
Leden van een politieke partij overwegen om een bekende Vlaming als lijsstrekker naar voor te schuiven tijdens de volgende verkiezingen. Om te bepalen welke kandidaat geschikt is, willen de partijleden een schatting van het aantal kiezers die deze kandidaat zullen steunen. De tijdsduur en de kosten om elke kiezer individueel te ondervragen liggen veel te hoog. Daarom worden willekeurig 400 kiezers geselecteerd. Wat is de populatie en wat is de steekproef?
**<u>Oplossing 1</u>**
Populatie = alle kiezers
Steekproef = de 400 geselecteerde kiezers



<u>**Oefening 2**</u>
Geef voor de volgende variabelen aan of deze een nominale, ordinale, absolute, interval- of ratioschaal heeft:
a. De speelduur van liedjes op Spotify;

**Ratioschaal**: want logische volgorde, verschil tussen twee uitkomsten heeft eenduidige betekenis, natuurlijk nulpunt maar er is keuze in meeteenheid (min, sec, etc. )	

b. De kleur van dahlia’s (bloemen);

**Nominale schaal**: want kenmerk kleur kan niet op een voor de hand liggende manier als een getal weergegeven worden.

c. De jaaromzet van bedrijven;

**Ratioschaal**: want logische volgorde, verschil tussen twee uitkomsten heeft eenduidige betekenis, natuurlijk nulpunt maar er is keuze in meeteenheid (euros, dollar, etc. ).

d. Het aantal sterren dat de moeilijkheidsgraad van Denksport puzzels aangeeft;

**Ordinale schaal**: want ordening, maar onderlinge verschillen hebben niet noodzakelijk dezelfde betekenis.

e. De hoogte boven de zeespiegel van wintersportdorpen.

**Ratioschaal**: want logische volgorde, verschil tussen twee uitkomsten heeft eenduidige betekenis, natuurlijk nulpunt maar er is keuze in meeteenheid (meter, cm, …)



**<u>Oefening 4</u>**
Beschrijf bij elk van de volgende voorbeelden de populatie en de steekproef. Beoordeel de keuze van de steekproef naar de criteria aselect en representatief.
a. De lijn wil de uurregeling van de buslijn Brugge – Oostende optimaliseren voor de reizigers die reeds de buslijn nemen. Daarom wordt er 7 dagen na elkaar een enquête afgenomen bij telkens 10 willekeurige reizigers verspreid over heel de dag.

b. De stad Brugge wil weten hoe allochtone inwoners denken over de politiediensten in hun stad. Een vragenlijst wordt opgesteld en door een politieagent op 250 adressen (lukraak onder de allochtone bevolking) aangeboden. Het gezinshoofd van het gezin wordt gevraagd de lijst in te vullen.



**<u>Oplossing 4</u>**
a. **Populatie**: de reizigers die reeds de buslijn Brugge – Oostende nemen. Steekproef: de 7 x 10 willekeurige reizigers 

**Representatief**: ja, de steekproef bevat voldoende elementen van de verschillende groepen in populatie Aselect: ja, elke reiziger heeft dezelfde kans om ondervraagd te worden.

b. **Populatie**: alle allochtone inwoners van Brugge Steekproef: de 250 gezinshoofden 

**Representatief**: nee, want niet alle groepen van de populatie zijn vertegenwoordigd, bijvoorbeeld allochtone vrouwen en kinderen. Aselect: nee, want niet elke allochtone inwoner heeft dezelfde kans ondervraagd te worden.



<u>**Oefening 6**</u>

In de groep TI-S1-G1 van 75 studenten was het gemiddelde op het deelexamen “Problem solving” 10,5. In TI-S1-G2 van 95 studenten was het gemiddelde 10,7. Wat is het gemiddelde over de twee klassen heen?

<u>**Oplossing 6**</u>
Om het gemiddelde over de twee klassen te berekenen, doen we alsof alle studenten van G1 de 10,5 behaalden en alle studenten van G2 de 10,7:

![image-20200106114947624](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200106114947624.png)

(**170** = 75 + 95)



<u>**Oefening 8**</u>
Men vraagt aan 15 beveiligingsspecialisten naar het aantal security audits dat ze dat jaar uitgevoerd hebben.
In een eerste enquête zijn de antwoorden als volgt:

![image-20200106122009802](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200106122009802.png)

Bereken het gemiddelde, mediaan, standaardafwijking en teken de boxplot.

𝑥̅=41,3333… 

Me = 34 

s = 20,6074…

**Kan handmatig maar met de rekenmachine is het gemakkelijker.** **=> STAT - EDIT en de lijst invullen. Daarna stat - calc - 1-VAR Stats**

![image-20200106122113248](https://raw.githubusercontent.com/Florianvdab/Wiskunde-Examen/master/image-20200106122113248.png)

Boxplot tekenen is **EZ** - Alles staat in die 1-VAR Stats.
