Esempio di conversione
======================

Obiettivo del documento
-----------------------

Questo documento fornisce degli esempi di formattazione del testo
compatibili fra i diversi formati, inclusi RST, DOCX, ODT, MD e HTML.

Allo stesso tempo, il file RST serve come guida alla sintassi del
formato [reStructuredText](http://docutils.sourceforge.net/rst.html).

Questo documento è parzialmente basato su [questo
esempio](https://raw.githubusercontent.com/jgm/pandoc/master/test/writer.rst).

Sezioni
-------

I titoli di sezione come quello qui sopra vanno strutturati in ordine
gerarchico. Un titolo di livello 1 dovrebbe essere seguito solo da
titoli di livello 2, non 3 o 4 per esempio.

Abbiamo sviluppato un filtro pandoc per correggere la struttura dei
titoli se dovesse servire.

### Livello 2

#### Livello 3

##### Livello 4

Sconsigliato per ragioni di leggibilità del testo.

Livello 1
---------

Questo è un paragrafo.

Questo è un altro paragrafo, separato dal precedente da una riga vuota.
I blocchi di testo non divisi da una riga vuota formano un unico
paragrafo.

Formattazione in linea
----------------------

Si definisce così la formattazione all'interno di un blocco di testo.
Ecco alcuni esempi.

### Corsivo

Ecco *due* esempi di *corsivo in una frase*.

### Grassetto

Il **grassetto** si formatta **con due asterischi**.

### Codice

Piccole porzioni di codice `<a href="#">Clicca qui</a>` possono essere
ottenute con i doppi apici.

### Apici e pedici

Testo^con apice^.

Testo~con pedice~.

### Link

Questo è [un URL](http://docs.italia.it/).

Un indirizzo email: [scrivici](mailto:a@b.it).

Un numero di telefono: [chiamaci](tel:+3902000000001).

Elenchi
-------

Gli elenchi puntati si creano con il trattino.

-   uno
-   due
-   tre

Gli elenchi numerati si creano con il numero seguito da un punto.

1.  primo
2.  secondo
3.  terzo

Autonumerazione degli elenchi.

1.  Qui
2.  Quo
3.  Qua
    1.  Paperino

### Elenchi annidati

-   tab
    -   tab
        -   tab

Oppure:

1.  primo
    -   alfa
    -   beta
    -   gamma
2.  secondo
    -   alef
    -   bet
    -   ghimel

Formattare blocchi di testo
---------------------------

I blocchi di testo si possono formattare usando il menu a tendina
relativo allo stile negli editor WYSIWYG.

### Formattare il codice

    Questo testo ha lo stile “Source Code”, da usare per gli esempi di codice sorgente

In alternativa, è possibile specificare il linguaggio del codice.

``` {.sourceCode .html}
<a href="#">clicca qui</a>
```

Aggiungere il numero della riga.

``` {.sourceCode .html}
<a href="#">clicca qui</a>

<a href="#">clicca anche qui</a>
```

### Citazioni

Questo è un blocco formattato come citazione.

> Frase molto importante di una persona molto famosa.

Paragrafo successivo.

Immagini e tabelle
------------------

### Immagine (senza didascalia)

![Testo alternativo. Luna](media/image1.jpeg){width="2.08403in"
height="2.27847in"}

### Figura (con didascalia)

La formattazione centrata non viene resa correttamente in DOCX e ODT.

![Didascalia della figura, separata dalle opzioni precedenti da una riga
vuota.](media/image1.jpeg){.align-center width="2.08403in"
height="2.27847in"}

### Tabella (senza didascalia)

  ----- ----- -----
  H1    H2    H3

  A1    A2    A3

  B1    B2    B3
  ----- ----- -----

### Tabella (con didascalia)

  ----- ----- -----
  H1    H2    H3

  A1    A2    A3

  B1    B2    B3
  ----- ----- -----

  : Didascalia della tabella

Note a piè di pagina
--------------------

Una nota alla fine di una riga[^1].

-   La nota si può mettere anche all\'interno di un elenco[^2].

[^1]: Nota importante.

[^2]: Altra nota importante.
