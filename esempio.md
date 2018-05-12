Esempio di conversione

Obiettivo del documento
=======================

Questo è un documento di esempio che potete usare per capire come
funziona RST. A fianco di questo file si trova lo stesso documento
convertito in altri formati. Confrontando I files potete capire come
usare RST per ottenere lo stile desiderato. Il titolo sopra è di primo
livello, ora possiamo introdurre un titolo di secondo livello per
entrare più in dettaglio

Formattazione in linea
======================

Si dice così la formattazione all'interno di un blocco di testo, vediamo
alcuni esempi

Corsivo
-------

Ecco *due* esempi di *corsivo*

Grassetto
---------

Il **grassetto** si formatta **così**

Link
----

Questo è [un link](http://docs.italia.it/)

Formattare blocchi di testo
===========================

I blocchi di testo si possono formattare usando il menu a tendina
relativo allo stile

Formattare il codice
--------------------

    Questo testo ha lo stile “Source Code”, da usare per gli esempi di codice sorgente

Citazioni
---------

Questo è un blocco formattato come citazione

Immagine
--------

![image0](media/image1.jpeg){width="2.08403in" height="2.27847in"}

Tabella
-------

  ----- ----- -----
  H1    H2    H3

  A1    A2    A3

  B1    B2    B3
  ----- ----- -----

Una nota sui titoli
===================

I titoli di sezione come quello qui sopra vanno strutturati in ordine
gerarchico. Un titolo di livello 1 dovrebbe essere seguito solo da
titoli di livello 2, non 3 o 4 per esempio. Abbiamo sviluppato un filtro
pandoc per correggere la struttura dei titoli se dovesse servire
