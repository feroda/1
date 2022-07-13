# Basic happy IOT device

Nel progetto [1 miliardo per la libertà](https://github.com/feroda/1) si intende implementare un sistema di monitoraggio della felicità.

Ma cosa si intende di preciso e come raggiungere questo obiettivo?

Lo stile del progetto è di rimanere semplici e stimolare le persone perché conviene ed è bello partecipare.

In questo caso l'obiettivo del percorso territoriale punta ad aumentare la felicità
e se questo obiettivo fosse condiviso ogni cittadino sarebbe interessato a monitorare la propria felicità.

Ma come? Ognuno è responsabile della propria felicità. La felicità è un sentimento. Di solito privato perché
non potremo mai condividere pienamente le sensazioni che proviamo esternamente.

"Per quanto mi identifichi col battito di un altro, sarà sempre attraverso questo cuore" (cit. Jovanotti: "Mezzogiorno")

Se fossimo interessati a monitorare questa sensazione pensiamo basterebbe un dispositivo casalingo
con 3 pulsanti da premere la sera dopo una giornata vissuta:

- Sono meno felice di stamattina: -1
- Sono felice allo stesso modo: 0
- Sono più felice di stamattina: +1

Non si ritiene necessario un indicatore assoluto in percentuale di quanto ci riteniamo felici in un istante t iniziale.

## Il dispositivo di monitoraggio della felicità

### Hardware base: 3 pulsanti

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

