FANTAPROF — SITO + BACKEND CON CODICI D'INVITO

CONTENUTO
- index.html: sito con pannello per creare una lega e unirsi tramite codice.
- config.js: URL backend da impostare dopo il deploy.
- backend/: server Node.js per account, stato, creazione leghe e inviti.

PASSAGGI NECESSARI
1. Pubblica la cartella backend su hosting Node.js (Node 20+), build: npm install, start: npm start.
2. Imposta JWT_SECRET con stringa casuale lunga (almeno 32 caratteri).
3. Configura DATA_FILE su disco persistente, es. /var/data/fantaprof.json.
4. Copia l'URL HTTPS del backend in config.js al posto del placeholder.
5. Carica index.html e config.js nella root di GitHub Pages.
6. Prova con due account distinti: uno crea la lega e l'altro usa il codice.

IMPORTANTE: il backend va deployato separatamente; GitHub Pages non esegue Node.js. Il vecchio server Emergent non viene modificato da questo ZIP. I permessi di squadra e la migrazione dei dati esistenti richiedono test prima di invitare tutti i giocatori.

NOTA IMPORTANTE SULLA CONDIVISIONE: la pagina Tutte le squadre mostra le squadre già presenti nello stato caricato dall’app. La sincronizzazione del gameplay tra account diversi (acquisti, eventi, formazioni e aggiornamenti live) non è ancora completa in questo pacchetto: i codici d’invito da soli non bastano. Non invitare tutti prima di testare questa parte con due account.
