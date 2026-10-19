FANTAPROF - PACCHETTO PER GITHUB PAGES

FILE
- index.html : il gioco completo (login con nome utente e password, salvataggio online)
- config.js  : indirizzo del server Fantaprof

COME PUBBLICARE
1. Carica index.html e config.js nella root del repository GitHub (sostituisci il vecchio index.html).
2. Elimina dal repository i vecchi file non più usati: sw.js, supabase-config.js, fantaprof-cloud.sql, manifest.webmanifest.
3. Dopo aver fatto Publish > Deploy su Emergent, apri config.js e metti l'indirizzo della app pubblicata
   (es. https://nome-app.emergent.host) al posto di quello di anteprima.
4. Attiva GitHub Pages (Settings > Pages > branch main, cartella root) e condividi il link.

NOTE
- Gli account e i dati sono salvati sul server Fantaprof, non su Supabase.
- Il link di anteprima nel config.js funziona solo per i test: per un link stabile usa l'indirizzo del deploy.
