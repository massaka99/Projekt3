# Projekt3

Dette projekt er gennemført som en del af kurset: "Semesterprojekt 3" @ Aarhus Universitet.

Formålet med projektet er at lave et karaokesystem, hvor et inputsignal korreleres med et foruddefineret signal, og en score beregnes. Den består af 2x RP'er og en PSoC-enhed og en Behringer UM2-lydgrænseflade. Hovedsystemet kører på en RPi4, med RPiOS installeret på den. Det er her Logic Unit og UI er til stede. Dataene håndteres af en RPiZero, der fungerer som en server. Formålet var at efterligne et cloudmiljø, hvor data gemmes eksternt og trækkes og skubbes efter behov af hovedsystemet. Derfor blev der lavet en ClientSocket-klasse, som er en grænseflade for hovedenheden til at interagere med serveren og skabe let tilgængelige data til hovedenheden. Indgangssignalet behandles på PSoC'en og sendes videre til hovedenheden i form af en WAV-fil, som derefter korreleres på RPi4'en. En intuitiv brugergrænseflade blev også designet og implementeret.

For at lære mere henvises til PDF'en i projektets repo, som er en gennemgående rapport om vores proces, udvikling, ansvar og resultater ved implementering af det ovenfor beskrevne system.
