# Primo avvio

- Registrazione utente **5**

  - ui, form di registrazione
  - ui, linee guida per l'accesso
  - ui, brevissima landing page
  - api, endpoint registrazione
  - api, modello/tabella db
  - api, registrazione e setup con passport local

- Login utente **5**

  - ui, form di accesso
  - ui, link a registrazione
  - api, endpoint accesso
  - api, login passport local

- Definizione nuovo magazzino **2**
  - ui, lista magazzini
  - ui, inserimento dati generali (nome, indirizzo)
  - ui, inserimento dimensioni
  - ui, inserimento supporti (scaffali, per terra, ceste, pallet...)
  - ui, inserimento mezzi di trasporto (muletti, robot, a piedi)
  - api, endpoint caricamento dati (uno solo)
  - api, salvataggio entità su db

# Utilizzo magazzino

- Scansione codice e registrazione paccco **3**

  - ui, lista pacchi presenti
  - ui, nuovo pacco/generalità
  - ui, scansione codice/SKU singolo
  - ui, inizio caricamento CSV
  - ui, completamento caricamento CSV -> verifica campi ed elenco pacchi in stand-by
  - api, endpoint nuovo pacco singolo
  - api, endpoint nuovo pacco da CSV
  - api, gestione errori CSV
  - api, salvataggio entità su db
  - api, avvio calcolo

- Calcolo posizionamento ottimale **1**

  - ui, panoramica isole
  - ui, avviso creazione nuova isola/assegnazione a isola
  - ui, guida al posizionamento
  - ui, pagina di conferma
  - ui, mappa del magazzino
  - api, endpoint calcolo -> selezione isola esistente o richiamo endpoint di creazione
  - api, endpoint isole -> analisi caratteristiche
  - api, endpoint isole -> salvataggio su db
  - api, salvataggio posizione collo su db

- Scarico colli/modifica **4**
  - ui, selezione isola da mappa
  - ui, selezione isola da elenco
  - ui, selezione collo da elenco
  - ui, ricerca collo
  - ui, pagina di scaricamento
  - ui, scansione codice
  - ui, proposta riposizionamento
  - api, ricerca collo
  - api, endpoint scaricamento
  - api, rimozione da db/status=uscito
  - api, ricalcolo posizione interna all'isola di altri colli
  - api, mail/notifica di altro tipo per scaricamento (stile negozio online)
