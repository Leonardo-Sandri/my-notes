La gestione della memoria in un sistema operativo può avvenire attraverso l'uso di **partizioni fisse** o **partizioni variabili**, ognuna con caratteristiche, vantaggi e svantaggi distinti.

## Partizioni Fisse

Le **partizioni fisse** sono suddivisioni della memoria in un numero predeterminato di aree di dimensioni fisse. Ogni partizione è assegnata a un processo e, se un processo è più piccolo della partizione, la porzione non utilizzata rimane sprecata, causando **frammentazione interna**. Questo sistema è semplice da implementare e richiede un basso overhead per la gestione delle partizioni. Tuttavia, presenta alcuni svantaggi:

- **Spreco di memoria**: La dimensione fissa delle partizioni può portare a una cattiva allocazione della memoria, specialmente se i processi hanno dimensioni variabili.


## Partizioni Variabili

Le **partizioni variabili**, al contrario, permettono una maggiore flessibilità. In questo modello, la memoria è inizialmente considerata come un'unica grande partizione libera. Quando un nuovo processo viene caricato, viene creata una partizione della dimensione esatta necessaria per quel processo. Questo approccio riduce significativamente la frammentazione interna poiché ogni partizione è dimensionata in base alle esigenze del processo. Tuttavia, le partizioni variabili comportano anche alcuni problemi:

- **Frammentazione esterna**: Questa si verifica quando ci sono spazi liberi nella memoria che non possono essere utilizzati perché sono troppo piccoli per soddisfare la richiesta di un nuovo processo, anche se la loro somma sarebbe sufficiente.
- **Gestione complessa**: La necessità di tenere traccia delle partizioni libere e allocarle dinamicamente rende la gestione più complessa rispetto alle partizioni fisse.


Per tornare alla home: [[content/index|index]]
