# Primo avvio

- Registrazione utente **P5**

  - ui, form di registrazione -> no username, conferma password **2**
  - ui, linee guida per l'accesso e brevissima landing page **2**
  - api, endpoint registrazione **1**
  - api, modello/tabella db -> nome, cognome, azienda, nomeutente (generato), email, password **5**
  - api, registrazione e setup con passport local **5**

- Login utente **P8**

  - ui, form di accesso **2**
  - ui, link a registrazione **1**
  - api, endpoint accesso **1**
  - api, login passport local **2**

- Definizione nuovo magazzino **2**
  - ui, lista magazzini con stato, percentuale riempimento e collegamento a crea nuovo **5**
  - ui, inserimento dati generali (nome, indirizzo) **2**
  - ui, inserimento dimensioni **2**
  - ui, inserimento supporti (scaffali, per terra, ceste, pallet...) **3**
  - ui, inserimento mezzi di trasporto e relative dimensioni, elevazione massima (muletti, robot, a piedi) **3**
  - api, endpoint caricamento dati (uno solo) **1**
  - api, salvataggio entità su db e inizializzazione coda stand-by **5**

# Utilizzo magazzino

- Scansione codice e registrazione paccco **P3**

  - ui, lista pacchi presenti **3**
  - ui, nuovo pacco/generalità **2**
  - ui, caratteristiche (fragile, dimensioni, impilabile, tipo) **2**
  - ui, inserimento (se presente) data uscita **1**
  - ui, lista stand-by e accetta/rifiuta/attesa **3**
  - ui, scansione codice/SKU singolo **5**
  - ui, inizio caricamento CSV **2**
  - ui, completamento caricamento CSV -> verifica campi ed elenco pacchi in stand-by **5**
  - api, endpoint nuovo pacco singolo **2**
  - api, endpoint nuovo pacco da CSV **3**
  - api, endpoint lista stand-by **3**
  - api, gestione errori CSV **3**
  - api, salvataggio entità su db **8**
  - api, avvio calcolo **2**

- Calcolo posizionamento ottimale **P1**

  - ui, panoramica isole **8**
  - ui, avviso creazione nuova isola/assegnazione a isola **2**
  - ui, suddivisione griglia isola **5**
  - ui, guida al posizionamento e mezzo di trasporto **2**
  - ui, pagina di conferma **2**
  - ui, mappa del posizionamento interno dell'isola **8**
  - api, definiziona griglia interna basata su molteplicità prodotti, dimensioni e caratteristiche **8**
  - api, priorità di uscita se data presente **8**
  - api, endpoint calcolo -> selezione isola esistente o richiamo endpoint di creazione **8**
  - api, endpoint isole -> analisi caratteristiche **5**
  - api, endpoint isole -> salvataggio su db **5**
  - api, salvataggio posizione e id isola collo su db **5**

- Scarico colli/modifica **P4**
  - ui, selezione collo da elenco **3**
  - ui, ricerca collo **2**
  - ui, pagina di scaricamento **5**
  - ui, scansione codice **5**
  - ui, proposta riposizionamento (accetta/rifiuta) **8**
  - api, ricerca collo **8**
  - api, endpoint scaricamento **5**
  - api, rimozione da db o inserimento status in coda **5**
  - api, gestione coda uscita **8**
  - api, gestione archivio **8**
  - api, ricalcolo posizione interna all'isola di altri colli e avvio calcolo **5**
  - api, mail/notifica di altro tipo per scaricamento (stile negozio online) **5**
