# Eco Ita
### Creato da Samuele Max, Davide Piaggi, Daniele Kim, Simone Kristo, Giuseppe Vaccaro e Tamer Qaddura

## Sito Web
Abbiamo creato questo sito come parte del progetto di educazione civica sui prodotti made in italy creati a partire dagli scarti industriali. Purtroppo abbiamo avuto 3 ore in meno per lavorare, quindi il sito non è completamente finito e non è stato reso responsive (ovvero non funziona sui dispositivi mobili, ma solo sui computer o sui tablet grandi). Si può visualizzare a questo link: [https://samuelemax.github.io/eco-ita/](https://samuelemax.github.io/eco-ita/).

## Come clonare
Requisiti:
- NodeJS 20

1. Clonare il repository usando git clone `git clone https://github.com/SamueleMax/eco-ita.git`
2. Entrare nella cartella clonata ed eseguire `npm i` per installare le dipendenze necessarie
3. Eseguire `npm run dev` oppure `npm run dev -- --host` per poter accedere al sito da qualunque dispositivo connesso in LAN

## Struttura delle cartelle
Il sito è stato creato in HTML e CSS utilizzando [Astro](https://astro.build/), un framework NodeJS che offre alcune funzionalità come la possibilità di creare dei componenti riutilizzabili e l'ottimizzazione automatica delle immagini. Astro è stato configurato per fornire dei file statici HTML e CSS in output, quindi non c'è bisogno di un server NodeJS ma basta uno spazio hosting qualunque. Il repo è stato configurato in modo che ad ogni push venga automaticamente fatta la build del sito, che si può fare manualmente in locale con `npm run build`.

- public: i file in questa cartella verranno messi così come sono al root del sito; attualmente c'è la favicon e alcune immagini che non devono essere ottimizzate
- src/assets: le immagini del sito che verranno ottimizzate e convertite in webp da Astro
- src/components: componenti riutilizzabili scritti in html e css
- src/layouts: il file di layout che contiene le dichiarazioni html, head, e altre cose globali per tutte le pagine
- src/pages: le pagine del sito
