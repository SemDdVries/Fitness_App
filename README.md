# Fitness_App
Fitness App met deze functionaliteiten tot nu toe:
Hoofdfunctionaliteiten
1. Workouts bijhouden
    - Naam kunnen geven per workout
    - elke workout moet een knop zijn waarop je kan klikken om de specifieke dingen te kunnen zien (welke oefening, welk gewicht etc.)
    - Sectie toevoegen waarin beginners voorbeelden kunnen zien van de workout (hoe gaan we dit krijgen?)
    - Automatisch progressieplan kunnen maken op basis van gewicht en historie, zou een coole kans kunnen zijn om hier AI voor te gebruiken. 

2. Agenda
    - Per week alles automatisch in kunnen plannen
    - Workouts moeten hergebruikt kunnen worden en een naam kunnen krijgen
    - Duidelijk aangeven of de training voltooid is, half voltooid is of nog niet begonnen
    - Mensen toe kunnen voegen aan je rooster?

3. Social media
    - Volgers een optie maken zodat mensen je workout schema kunnen volgen of kopen.
    - Groepen maken waarop verschillende disciplines met elkaar kunnen communiceren (powerliften, bodybuilding, shredding, bulking, calesthenics) 
    - Shorts/foto's kunnen posten om volgers te krijgen.

4. Voedseltracking
    - Zorgen dat mensen zelf hun macro's bij kunnen houden
    - Betaalde optie om voedselschema's te kunnen kopen van bekende mensen/AI voedselschema's gebaseerd op je calorie intake + benodigde macro's. 
    - Voedsel op kunnen zoeken zodat ze niet bij elk voedselstuk in hoeven te vullen hoeveel calorien ze denken dat er in zit. 

5. Shop
    - Afdelingen maken, waaronder kleding, trainingsschema's en maaltijden (complete maaltijden die bezorgd worden/voedingsschema's)
    - Kleding; kan elk sport kleding merk zijn
    - Trainingsschema's: we kunnen hierbij een gratis sectie doen waar iedereen zijn/haar trainingsschema kan delen (zoals je op spotify met iedereen je playlist kan delen) en dan een betaalde optie doen voor influencers. 
    - Maaltijden; uiteraard betaald. Betaalde afdeling doen voor influencers en als we geluk hebben nog bezorgde sportmaaltijden aanbieden (zoals musclefood bijvoorbeeld). 

6. Consistency + competitie
    - Zorgen dat mensen blijven terugkomen door een streak te laten zien. Voor elke complete trainingsweek krijgen ze voor 1 dag een freeze streak bijv. Dit zouden we nog kunnen onderbouwen met wetenschappelijke kennis (Een streak laten zien verbeterd de kans met ...% dat je blijft terugkomen). 
    - Deze streak sociaal maken waardoor een langere streak aan de buitenwereld getoond kan worden. 
    - Competitie creeren door een database van mensen te verzamelen, en deze gegevens gebruiken zodat je jezelf ermee kan vergelijken. Voorbeeld: we hebben 100 gebruikers, waarvan het bench gemiddelde op 100kg ligt. Als ik 140kg kan benchen, zit ik in de top 10% sterkste benchers in onze app. Hierdoor maken we de app competitief en willen mensen steeds sterker worden, waardoor ze terug blijven komen. 

Grote vraagstukken:
- Hoe zorgen we ervoor dat we kunnen controleren of workouts ook echt worden voltooid? of wordt dit op goed vertrouwen? 
    - In het begin duidelijk maken dat deze app op goed vertrouwen is en dat liegen geen nut heeft met een disclaimer. Uiteindelijk kunnen we in grote commerciele sportscholen een scanner maken waardoor mensen aan kunnen duiden dat ze bij de sportschool zijn geweest door deze QR-code te scannen. En als je er al bent om de QR-code te scannen kan je net zo goed gaan toch?? Ook kunnen we voor mensen die beweren in de top 1% te zitten met hun lifts vragen om videos op te sturen waarin ze dit bewijzen waarna wij bij de lift bij kunnen zetten dat het een "certified lift" is. Als we dit kunnen automatiseren met AI zijn we binnen want dan hoeft dit niet per persoon gecontroleerd te worden en kan iedereen "certified lift" bij oefeningen krijgen. 
- Hoe zorgen we ervoor dat mensen onze app gaan gebruiken i.p.v. andere social media?
    - We moeten eerst zorgen dat we gebruikers krijgen door de app heel breed (veel functies), maar ook heel toegankelijk te maken (beginners guides, simpele en interactieve UI) zodat mensen het gaan gebruiken. Als dit eenmaal lukt kunnen we proberen via gesponserde atleten de influencer sectie uit te breiden waarna we ervoor kunnen zorgen dat er genoeg videos op staan dat zoveel mogelijk sporters hierop gaan posten, waardoor het een echte social media wordt. 
- Wat gaan de betaalde opties worden en wat niet?
  
Stappenplan:

1. App opzetten. Uitzoeken hoe we een app gaan maken, hoe Native React werkt en hoe we aan de app zelf kunnen werken. 
2. Inlogsysteem creeren voor de users. Eerst nog simpel maken door username en wachtwoord aan te laten maken, waarna ze eventueel een profielfoto kunnen toevogen. Uiteindelijk kunnen we hier inloggen via Google of whatever account aan toevoegen. Hierbij moet ook een profiel worden aangemaakt waarbij mensen hun sportschool waar ze trainen kunnen toevoegen (dit kunnen gebruikers prive houden vanwege privacy redenen) en gegevens in kunnen vullen omtrent gewichten per oefening. Dit zal automatisch moeten worden vernieuwd wanneer ze aangeven in een trainingsschema dat ze een hoger gewicht hebben gedaan dan de PR aangegeven in deze sectie. 
3. Met Native React proberen te beginnen met de eerste functionaliteiten. Het belangrijkste onderdeel is het kunnen toevoegen van workouts, deze een naam kunnen geven en deze op kunnen slaan. Dit kunnen we eerst heel simpel maken door gwn simpelweg een knop te creeren waarop mensen kunnen drukken zodat ze een nieuw schema kunnen maken (een + knop ergens rechtsbovenin). Als ze hierop klikken komen ze in een nieuw scherm waarin ze het schema een naam kunnen geven of leeg kunnen laten, waarna we de workout "Workout ..." noemen, waarbij de ... vervangen wordt door 1, 2, 3 optellend. Zodra ze een naam hebben gekozen komen ze in een nieuw scherm waarbij ze met een nieuwe + knop oefeningen toe kunnen voegen. Zodra zo op deze knop klikken komt er een zoekmenu tevoorschijn waarbij ze naar bestaande oefeningen kunnen zoeken, of kunnen ze ervoor kiezen de oefening zelf een naam te geven. Zodra ze dit hebben gedaan kiezen ze de hoeveelheid sets en reps die ze willen doen + hoeveel gewicht ze willen voltooien. Nadat ze dit hebben gedaan wordt dit als doelstelling neergezet voor de oefening. Na elke oefening kunnen ze nog echt invullen wat ze gedaan hebben, zodat ze in hun agenda altijd terug kunnen vinden wat het doel was en wat ze hebben behaald (meer of minder reps/sets/gewicht). Hier kunnen we uiteindelijk nog een betaalde optie inzetten waarbij de stap met sets, reps en gewicht wordt geautomatiseerd naar aanleiding van gebruikers gewicht en PR op de oefening (70% van PR moet je voor 10 reps doen bijvoorbeeld, dit kunnen we nog helemaal uitzoeken maar niet belangrijk voor het begin.) 
4. Mij lijkt het handig om met een app te beginnen die we zelf zouden gebruiken, dus een mooi schema maken met een duidelijke agenda waarin je je eigen workouts kan toevoegen en een optie maken om ze per een bepaald aantal dagen te herhalen. 
Voorbeeld: Ik wil een schema van chest+tricep, rug+bicep, benen+schouders en een dag rust. De gebruiker moet dan in kunnen vullen hij dit schema wilt beginnen op maandag 1 januari, de rug+bicep dag op 2 januari, benen+schouders op 3 januari en rustdag op 4 januari. Nu moet de gebruiker ook kunnen kiezen dat elke trainigsdag om de 4 dagen moet herhalen, waardoor in het schema duidelijk staat dat er op 5 januari weer chest+tricep traindag is, 6 januari rug+bicep etc. 
5. Zodra dit werkt een mooie interface creeren waardoor de agenda overzichtelijk is, duidelijk is welke workouts je wel/niet hebt gedaan, en dat het duidelijk is welke workout je wanneer hebt en misschien zelfs toevoegen hoelaat je deze workout wilt gaan doen. het duidelijk maken van of je een workout wel of niet hebt gedaan kunnen we simpelweg gewoon met rood (niet gedaan), oranje (niet volledig voltooid) of groen (volledig voltooid) aanduiden. Het duidelijk maken welke workout je hebt kunnen we doen aan de hand van de naam die je in het schema tabblad hebt gekozen te vertonen in de agenda. 
6. Ook lijkt het me leuk dat je progressie foto's kan delen via je eigen profiel, waardoor je prive maar ook publiek kan laten zien welke voortgang je maakt in je sporten. Op deze manier houden we de app nog interactiever en kunnen mensen ook makkelijk terugzien hoe goed ze bezig zijn geweest. We kunnen dit zelfs toevoegen aan de kalender zodat het ook duidelijk wordt op welke dag dit was zodat we eventueel automatische flashbacks kunnen toevoegen. 
