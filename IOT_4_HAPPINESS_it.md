# IOT 4 Happiness

Nel progetto [1 miliardo per la libertà](https://github.com/feroda/1) si intende implementare un sistema di monitoraggio della felicità.

Ma cosa si intende di preciso e come raggiungere questo obiettivo?

Lo stile del progetto è di rimanere semplici e stimolare le persone perché conviene ed è bello partecipare.

In questo caso l'obiettivo del percorso territoriale punta ad aumentare la felicità
e se questo obiettivo fosse condiviso ogni cittadino sarebbe interessato a monitorare la propria felicità.

Ma come? Ognuno è responsabile della propria felicità. La felicità è un sentimento. Di solito privato perché
non potremo mai condividere pienamente le sensazioni che proviamo esternamente.

"Per quanto mi identifichi col battito di un altro, sarà sempre attraverso questo cuore" (cit. Jovanotti: "Mezzogiorno")

## PERSONAS

Procediamo ad un'analisi *customer centric* della piattaforma definendo alcune PERSONAS.

### Orlando: il 68ino sindacalista

Ha sempre speso il suo impegno con serietà e orientamento etico per i territori.

Usa il sistema per contribuire alla realizzazione di un indicatore territoriale. Inizialmente preferisce non perderci troppo tempo, ma pian piano si interessa maggiormente ai dettagli tecnici dato che per anni ha risolto problemi di formattazione di PC agli amici.

### Roberta: la funzionaria curiosa
Si interessa della situazione cittadina.

Usa il sistema per capire come è felicità riguardo ai luoghi e ai canali.

### Mariola: la domestica girandolona

Usa il sistema per capire come è felicità riguardo ai luoghi e ai canali. Le interessano le persone

### Matteo: il neodiplomato in cerca di avventure

A Matteo interessa ricevere segnalazioni di attività in base alle proprie segnalazioni di felicità sui CANALI che segue.

### Valerio: lo studente hacker

A Valerio interessa particolarmente la piattaforma open perché vuole autocostruirsi il dispositivo di segnalazione della felicità e capire come funziona il protocollo di comunicazione per portarlo al limite delle sue potenzialità ed eventualmente scoprire qualche falla di sicurezza

### Giovanna: la dipendente motivata

A Giovanna interessa esprimere la propria felicità sui CANALI aziendali che il suo capo ha attivato per la propria azienda (**GRUPPO**)

### Flavio: l'imprenditore rinomato

A Flavio interessa la possibilità di definire alcuni CANALI per la propria azienda (GRUPPO) in modo da capire il sentimento dei propri dipendenti rispetto ad essi.

A Flavio interessa inoltre capire nel territorio il sentimento rispetto agli stessi CANALI siano essi in altri GRUPPI oppure senza gruppo (utenti finali).

## Cosa serve per raggiungere questo scopo?

- Un dispositivo (**DEVICE**) assegnato all'utente per inviare il suo livello di felicità o una app (**APP**)
- Una piattaforma (**CLOUD**) che aggreghi i dati provenienti dal DEVICE e mostri gli indicatori di felicità attraverso:
  - una mappa per territori
  - una mappa per gruppi
  - una mappa per categorie (**CANALI**) [non tutti gli utenti valutano canali specifici]
  - una mappa per relazioni tra i CANALI [per le valutazioni ricevute su canali]
  - [opzionale] una mappa per tipologie dei soggetti che partecipano al monitoraggio
- Un'interfaccia grafica (**UI**) che consenta una piacevole esperienza utente (**UX**) all'utente
- Un protocollo di comunicazione DEVICE/CLOUD e UI/CLOUD (**API_CLOUD**)

## HAPPY IOT UI per la visualizzazione

[TODO]: inserire una mappa con i cuori di diverse dimensioni e colori

In alto la possibilità di filtrare per una o più categorie e uno o più gruppi. Il filtro sarà applicato contestualmente al territorio visualizzato.

In alto a destra le informazioni dell'utente o del DEVICE con i PUNTI/BADGE associati.

A scomparsa le news/i tasks/le challenge relative/i ai CANALI e i TERRITORI. 

## L'utente vede e intende partecipare (PROFILI)

La registrazione alla piattaforma riveste un aspetto di fondamentale importanza considerato che la felicità non può prescindere dalla libertà di decisione da parte dell'individuo su come partecipare al monitoraggio. 

A seconda delle PERSONAS definite sopra, si ipotizzano diverse modalità di registrazione, cui corrispondono differenti profili di utenza.

Chi vorrà abilitare un utente potrà farlo con SPID, chi vorrà abilitare solamente un DEVICE, senza associarlo alla propria persona, dovrà comunque associarvi uno SMARTPHONE per la conferma.

### La registrazione di Flavio

Flavio è un imprenditore che vuole registrare la sua azienda come GRUPPO associando ad essa uno o più CANALI perciò si registrerà con un UTENTE, vi assocerà uno SMARTPHONE e opzionalmente uno o più DEVICE.

Con il suo UTENTE potrà creare il GRUPPO azienda.

Perciò avrà un profilo di GESTORE_DI_GRUPPO (permesso che probabilmente avranno tutti, ma non tutti useranno)

### La registrazione di Giovanna

Giovanna è una dipendente che vuole partecipare a livello di TERRITORIO e di azienda (GRUPPO).

Per questo anch'essa dovrà disporre di un UTENTE, con associato uno SMARTPHONE e se lo vorrà uno o più DEVICE

### La registrazione di Orlando

In un primo momento Orlando non vuole far altro che contribuire al territorio perciò recupererà un DEVICE o se lo autocostruirà. Poi lo registerà nel CLOUD e vi potrà associare il proprio SMARTPHONE

## HAPPY IOT CLOUD per l'aggregazione

Il sistema CLOUD è ciò che sta dietro per cui è il meno interessante ai fini di questo documento.

Il suo ruolo è quello di ricevere le segnalazioni di felicità e di smistare MESSAGGI (news, tasks, challenges) nei territori e nelle categorie di interesse.

Ciò implica il trattamento di Big Data e l'interazione con un sistema di AI per la riconducibilità dei MESSAGGI ai CANALI e ai TERRITORI.

## HAPPY IOT DEVICE per la segnalazione

Abbiamo pensato che per monitorare questa sensazione in modo semplice sia sufficiente un dispositivo con 3 pulsanti da premere la sera dopo una giornata vissuta:

- Sono meno felice di stamattina: -1 ![](https://via.placeholder.com/20x20/ee0000/000000?text=+)
- Sono felice allo stesso modo: 0 ![](https://via.placeholder.com/20x20/eeee00/000000?text=+)
- Sono più felice di stamattina: +1 ![](https://via.placeholder.com/20x20/7cfc00/000000?text=+)

Non si ritiene necessario un indicatore assoluto in percentuale per esprimere un valore quantitativo. Almeno inizialmente.

Il dispositivo può essere dotato di un display per la selezione del CANALE cui si intende attribuire il proprio indicatore di felicità.

### Hardware base: 3 pulsanti

Il dispositivo può anche essere autocostruito e sarebbe un ottimo esercizio da proporre nei PTOF degli ITIS del territorio nei corsi di Elettronica e di Informatica.

- Microcontrollore
- Pulsanti R,Y,G e cavetti
- Alimentazione power/batteria
- Led indicatori
- Connettività (WiFi o modem GSM o Ethernet)
- Case e serigrafia
- GPS

### Protocolli/API:

Anche questo è poco interessante, da rivedere. TODO

Vengono salvati: timestamp, valore, posizione GSM, token di autenticazione

- autenticazione? token

- invio a numero GSM
- invio via MQTT
- invio via HTTP
- invio via TCP