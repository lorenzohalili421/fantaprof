FANTAPROF — PWA INSTALLABILE (BASE DI LAVORO)

Questa cartella conserva la PWA ricevuta e include note per la futura integrazione online.

IMPORTANTE
- La PWA attuale salva ancora i dati in localStorage: non sincronizza tra dispositivi.
- La presenza di supabase-config.example.js NON significa che l'app sia già collegata.
- Le tabelle Supabase hanno RLS attiva ma non risultano policy configurate. Non aggiungere policy aperte a tutti.
- Non pubblicare questa versione come se fosse già un gioco online multiutente.

FILE
- index.html: app attuale
- manifest.webmanifest: impostazioni installazione PWA
- sw.js: service worker
- icons/: icone
- ONLINE_STATUS.txt: requisiti per il completamento sicuro
- supabase-config.example.js: esempio di configurazione non ancora collegato

PROSSIMI PASSI DI SVILUPPO
1. Disegnare/validare schema per account, leghe e ruoli.
2. Implementare autenticazione e backend sicuri per login con nome squadra e password.
3. Configurare policy RLS specifiche e funzioni server-side per operazioni riservate.
4. Collegare tutte le schermate al database, rimuovendo il salvataggio locale come fonte principale.
5. Testare autorizzazioni e sincronizzazione prima di pubblicare.

NON mettere mai chiavi secret/service_role nel codice del browser o in GitHub.
