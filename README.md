# Esercizio: **Carosello Mono Array**
nome repo: js-array-carousel

## **Consegna:**
Dato un array contenente una lista di cinque immagini, creare un carosello come nello screenshot allegato.
### **MILESTONE 1**
Per prima cosa, creiamo il markup statico: costruiamo il container e inseriamo un’immagine grande al centro: avremo così la struttura base e gli stili pronti per poterci poi concentrare solamente sull’aspetto logico.
### **MILESTONE 2**
Adesso rimuoviamo tutto il markup statico e inseriamo tutte le immagini dinamicamente servendoci dell’array fornito e un semplice ciclo for che concatena un template literal.
Tutte le immagini saranno nascoste, tranne la prima, che avrà una classe specifica che la renderà visibile.
Al termine di questa fase ci ritroveremo con lo stesso slider stilato nella milestone 1, ma costruito dinamicamente attraverso JavaScript.
### **MILESTONE 3**
Al click dell’utente sulle frecce, il programma cambierà l’immagine attiva, che quindi verrà visualizzata al posto della precedente.
### **BONUS 1:**
Aggiungere il **ciclo infinito** del carosello. Ovvero se è attiva la prima immagine e l’utente clicca la freccia per andare all’immagine precedente, dovrà comparire l’ultima immagine dell’array e viceversa.
### **BONUS 2:**
Aggiungere la visualizzazione di tutte le thumbnails sulla destra dell’immagine grande attiva, come nello screenshot proposto. Tutte le miniature avranno un layer di opacità scura, tranne quella corrispondente all’immagine attiva, che invece avrà un bordo colorato.
Al click delle frecce, oltre al cambio di immagine attiva, gestire il cambio di miniatura attiva.

---

#### Procedimento logico:

- creo un template delle mie immagini che hanno un display-none di default assegnato tramite una classe

- attraverso un indice gestico a chi levare e mettere la classe d-none

- creo i due bottoni, che nella versione statica dovranno vedersi o scomparire in base alla situzione, se nella condizione ciclo continuo, devo modificare l'indice del mio contatore per resettarlo

- per la thumbnails quando carico il template con js, per le immagini grandi, carico anche dei template di immagini più piccole, che avranno una classe active all'occorrenza
