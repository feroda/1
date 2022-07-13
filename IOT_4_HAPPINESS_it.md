# IOT 4 Happiness

Nel progetto [1 miliardo per la libertà](https://github.com/feroda/1) si intende implementare un sistema di monitoraggio della felicità.

Ma cosa si intende di preciso e come raggiungere questo obiettivo?

Lo stile del progetto è di rimanere semplici e stimolare le persone perché conviene ed è bello partecipare.

In questo caso l'obiettivo del percorso territoriale punta ad aumentare la felicità
e se questo obiettivo fosse condiviso ogni cittadino sarebbe interessato a monitorare la propria felicità.

Ma come? Ognuno è responsabile della propria felicità. La felicità è un sentimento. Di solito privato perché
non potremo mai condividere pienamente le sensazioni che proviamo esternamente.

"Per quanto mi identifichi col battito di un altro, sarà sempre attraverso questo cuore" (cit. Jovanotti: "Mezzogiorno")

## Cosa serve a questo scopo?

- Un dispositivo (**DEVICE**) assegnato all'utente per inviare il suo livello di felicità o una app (**APP**) che può essere:
- Una piattaforma (**CLOUD**) che aggreghi i dati provenienti dal DEVICE e mostri gli indicatori di felicità attraverso:
  - una mappa per territori
  - una mappa per categorie (**CANALI**) [non tutti gli utenti valutano canali specifici]
  - una mappa per relazioni tra i CANALI [per le valutazioni ricevute su canali]
  - [opzionale] una mappa per tipologie dei soggetti che partecipano al monitoraggio
- Un protocollo di comunicazione tra i DEVICE e il CLOUD

Perché l'ultimo punto CLOUD è opzionale?

Si lascia opzionale la possibilità di registrarsi al sistema e quindi diventare un utente non anonimo. Questo perché la felicità non può prescindere dalla libertà totale di decisione dell'individuo che potrà decidere via via il suo livello di accesso.

## Il DEVICE: un dispositivo di monitoraggio della felicità

Se fossimo interessati a monitorare questa sensazione nel modo più semplice possibile pensiamo basterebbe un dispositivo casalingo con 3 pulsanti da premere la sera dopo una giornata vissuta:

- Sono meno felice di stamattina: -1 [ROSSO]
- Sono felice allo stesso modo: 0 [GIALLO]
- Sono più felice di stamattina: +1 [VERDE]

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

Vengono salvati: timestamp, valore, posizione GSM, token di autenticazione

- autenticazione? token

- invio a numero GSM
- invio via MQTT
- invio via HTTP
- invio via TCP