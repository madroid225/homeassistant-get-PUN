# homeassistant-get-PUN
Piccolo flow node-red per homeassistant per recuperare il PUN giornaliero
La procedura presuppone che node-red sia installato come componente aggiuntivo su home assistant e che su node-red sia installato 
  node-red-contrib-home-assistant-websocket
La procedura gira ogni ora e la prima volta che riesce a scaricare il file memorizza tutte le ore in una variabile a livello di flow così ad ogni ora, dello stesso giorno non torna sul sito ma pesca il valore dalla memoria.
Ogni nuova ora salva il dato nel sensore così che sia utilizzabile nella plancia energia ed in ogni altro punto in cui serve.
Il dato è già normalizzato in €/kWh
