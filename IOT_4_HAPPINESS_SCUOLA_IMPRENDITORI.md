# IOT 4 Happiness @ Scuole Imprenditori

Si intende realizzare un proof-of-concept di IOT 4 Happiness per la **Scuola imprenditori**.

In questo caso la modellazione dati avviene sull'impostazione di [IOT_4_HAPPINESS.md](IOT_4_HAPPINESS.md).

Come interfaccia si intende utilizzare la potenzialità della chat/framework Telegram.

## UTENTE

- Nome
- Email
- Cell

(TODO: un URL via Cell deeplink Telegram)

## GRUPPO

1. Confartigianato Scuola Imprenditori `#chi:scuola-imprenditori`

## CANALI

Gli utenti saranno invitati in 3 canali corrispondenti ai moduli del corso:

1. Costi e Politica di Prezzo `#costo #prezzo #margine`
1. L'Analisi Finanziaria `#analisi-finanziaria`
1. Merito di Credito `#credito #banche`

In ogni canale sarà presente un bot utile per ricevere le risposte dei partecipanti e salvare l'indicatore di felicità nella piattaforma cloud.

## MESSAGGI

Questi saranno i messaggi che transitano nei canali

1. Sondaggio: è il tipo di messaggio principale con cui l'utente esprime la propria felicità in un certo istante t. Dovrebbe poterlo esprimere su ogni lezione del corso e con un commento. Riportiamo di seguito le lezioni:
  - 1a): La determinazione del costo del prodotto/servizio in periodi di forte aumento dei costi dei fattori produttivi;
  - 1b): I possibili orientamenti nella formulazione dei prezzi ed il valore percepito;
  - 1c): Il prezzo profittevole e le possibili differenziazioni di prezzo; 
  - 2a): Monitorare gli indici di allerta per prevenire criticità finanziarie;
  - 2b): Le principali leve operative e finanziarie per migliorare la situazione di liquidità a breve termine;
  - 2c): Analisi del cash flow e la gestione finanziaria connessa alla gestione economica;
  - 3a): Come migliorare il “Merito di Credito”: rendi efficace il rapporto con le Banche e definisci fino a che punto spingerti con i Prezzi di vendita;

Il risultato di questo sondaggio viene rimandato agli utenti e pubblicato sui CANALI relativi in forma aggregata.

Gli altri messaggi dovrebbero essere veicolati solamente se un utente ha aumentato la propria felicità relativamente al modulo (CANALE).

2. News
3. Tasks
4. Challenges

## PERSONAS

Approccio *Customer centric*

### Giuseppe: il neoimprenditore

Giuseppe ha avviato l'impresa ma più va avanti, più si rende conto che le competenze necessarie sono molte di più di quelle che si aspettava.

Giuseppe è interessato ad acquisire le competenze necessarie per poter gestire un'azienda a 360 gradi.

### Lucio: il microimprenditore

Lucio è un lupo solitario, corre dalla mattina alla sera dietro ad ogni scadenza che si presenta e ogni impatto esterno gli causa problemi. Ha difficoltà a delegare. Si pone la domanda: gli altri come fanno?

Partecipa alla scuola per:
- imparare ed identificare strumenti per definire priorità, scadenze ed esercitare un minimale controllo di gestione 
- imparare a delegare e verificare
- confrontarsi con gli altri imprenditori

### Federica: l'imprenditrice brillante

A Federica interessa la possibilità aumentare la felicità nella propria azienda e per questo vuole rilevare periodicamente il sentimento dei propri dipendenti.

Le interessa inoltre capire nel territorio il sentimento rispetto agli stessi temi che lei identifica nella propria azienda.