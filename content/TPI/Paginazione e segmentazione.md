La **paginazione** e la **segmentazione** sono due tecniche fondamentali utilizzate nella gestione della memoria nei sistemi operativi. Entrambe mirano a ottimizzare l'uso della memoria, ma operano in modi differenti e presentano vantaggi e svantaggi distinti.

## Paginazione

La paginazione consiste nel suddividere sia la memoria fisica che quella logica in blocchi di dimensioni fisse chiamati **pagine** (per la memoria logica) e **frame** (per la memoria fisica). Questo approccio consente di caricare solo le pagine necessarie in memoria, riducendo la necessità di contiguità fisica dei dati. **Caratteristiche principali:**

- **Dimensione fissa**: Le pagine e i frame hanno dimensioni identiche, il che semplifica la gestione della memoria.
- **Frammentazione interna**: Poiché le pagine hanno dimensioni fisse, può verificarsi uno spreco di spazio all'interno delle pagine non completamente utilizzate.
- **Trasparenza per il programmatore**: La paginazione è invisibile all'utente, poiché il sistema operativo gestisce automaticamente l'allocazione della memoria
## Segmentazione

La segmentazione, al contrario, divide la memoria in unità di dimensioni variabili chiamate **segmenti**, ognuno dei quali rappresenta una parte logica del programma, come funzioni o strutture dati. Ogni segmento ha un nome e una dimensione specifica. **Caratteristiche principali:**

- **Dimensione variabile**: I segmenti possono avere dimensioni diverse a seconda delle necessità del programma, consentendo un uso più efficiente della memoria.
- **Frammentazione esterna**: Poiché i segmenti possono avere dimensioni variabili, si può verificare uno spreco di spazio tra i segmenti, noto come frammentazione esternativa per gli sviluppatori poiché riflette la struttura logica del programma, facilitando la gestione delle strutture dati dinamiche.


Per tornare alla home: [[content/index|index]]
