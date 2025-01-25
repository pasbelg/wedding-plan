# wedding-plan
This repository contains the detailed planning timeline for our wedding. Please note that while the content is specifically tailored to our celebration, it has been intentionally kept generic to protect our personal information. If anyone stumbles upon this repo, feel free to use it as a template or source of inspiration for your own wedding or event planning.

The repository is in German, as it is more relevant to the people helping us organize our wedding, and we hope that the structure and organization of the planning will be helpful to them.

## Zeitlicher Ablauf
````mermaid
gantt
    dateFormat HH:mm
    axisFormat %H:%M
    Aufstehen : milestone, aufstehen, 08:00, 2m
    Kind fertig machen : kindFertig, after aufstehen, 10m
    Anziehen Braut (mit Trauzeugin) : frauFertig, after kindFertig, 2h
    Anziehen Bräutigam (mit Trauzeuge) : mannFertig, after kindFertig, 1h
    Warten auf Braut für First Look : wartenFL, after mannFertig, until firstLook
    First Look (im Hotelhof) : firstLook, after frauFertig, 15m
    section Standesamtliche Trauung
        Weg zum Standesamt (6 Minuten zu Fuß) : after firstLook, 10m 
        Termin Standesamt für Eheschließung : milestone, 11:00, 0m
        Eheschließung : ST, 11:00, 30m
    section Fotoshooting:
        Enspannen & Reden :  relax1, after ST, 45m
        Weg zurück zum Auto : wegAutoFS, after relax1, 10m
        Fahrt zum reservierten Shooting Ort : after wegAutoFS, 5m
        Fotoshooting : 1h
        Weg zu 2. Location : 10m
        2. Fotoshooting  : 1h
    section Freie Trauung
        Beginn freie Trauung : milestone, 15:00, 0m
        Einfinden der Gäste : einfindenFT, 15:00, 15:10
        Abspielen der Brautmarsch Musik : milestone, 15:10, 0mn
        Einzug der Braut (mit Vater): einzugFT, after einfindenFT, 2m
        Traurede : redeFT, after einzugFT, 10m
        Gelübte Braut : redeFrautFT, after redeFT, 10m
        Gelübte Bräutigam : redeMannFT, after redeFrautFT, 10m
        Trauung : trauung, after redeMannFT, 5m
        Ringübergabe : ring, after trauung, 2m
        Kuss & Jubel : after ring, 1m
        Abschlussrede & Anweisungen : 5m
    section Empfang
        Beginn Empfang : milestone, 16:00
        Erster Schnitt : 5m
        Freigabe für Festsaal : milestone, startFestsaal, 16:30,
    section Festsaal
        Einfinden im Festsaal: after startFestsaal, 20m
        Warten auf Essen : wartenEssen, after startFestsaal, until essenStart
        Beginn Essen : milestone, essenStart, 18:00,
        Musik läuft : milestone, after essenStart, 
        Gäste zum Buffet : runBuffet, after essenStart, 20m
        Gäste Essen : essen, after runBuffet, 1h
        Kling Kling Kling Schwester3 : milestone, klingSchwester3, after essen,
        Musik leiser drehen : musikLeiserSchwester3, after klingSchwester3, 1m
        Rede Schwester3 : after musikLeiserSchwester3, 20m
        Gäste Essen : after essen, 1h
        Warmes Essen Verfügbar : after essenStart, 21:00
````
