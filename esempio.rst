######################
Esempio di conversione
######################

Obiettivo del documento
=======================

Questo documento fornisce degli esempi di formattazione del testo compatibili
fra i diversi formati, inclusi RST, DOCX, ODT, MD e HTML. 

Allo stesso tempo, il file RST serve come guida alla sintassi del formato
`reStructuredText <http://docutils.sourceforge.net/rst.html>`_. 

Questo documento è parzialmente basato su `questo esempio <https://raw.githubusercontent.com/jgm/pandoc/master/test/writer.rst>`_.

Sezioni
=======

I titoli di sezione come quello qui sopra vanno strutturati in ordine
gerarchico. Un titolo di livello 1 dovrebbe essere seguito solo da
titoli di livello 2, non 3 o 4 per esempio. 

Abbiamo sviluppato un filtro pandoc per correggere la struttura dei titoli se
dovesse servire.

Livello 2 
----------

Livello 3
~~~~~~~~~

Livello 4
"""""""""

Sconsigliato per ragioni di leggibilità del testo.


Livello 1
=========

Questo è un paragrafo. 

Questo è un altro paragrafo, separato dal precedente da una riga vuota. 
I blocchi di testo non divisi da una riga vuota formano un unico paragrafo.

Formattazione in linea
======================

Si definisce così la formattazione all’interno di un blocco di testo. Ecco
alcuni esempi.

Corsivo
-------

Ecco *due* esempi di *corsivo in una frase*.

Grassetto
---------

Il **grassetto** si formatta **con due asterischi**.

Codice
------

Piccole porzioni di codice ``<a href="#">Clicca qui</a>`` possono essere
ottenute con i doppi apici.

Apici e pedici
--------------

Testo\ :sup:`con apice`. 

Testo\ :sub:`con pedice`.

Link
----

Questo è `un URL <http://docs.italia.it/>`__.

Un indirizzo email: `scrivici <mailto:a@b.it>`_.

Elenchi
=======

Gli elenchi puntati si creano con il trattino.

- uno

- due

- tre

Gli elenchi numerati si creano con il numero seguito da un punto.

1. primo

2. secondo

3. terzo

Autonumerazione degli elenchi.

#. Qui

#. Quo

#. Qua

   #. Paperino

Elenchi annidati
----------------

- tab
  
  - tab

    - tab

Oppure:

1. primo

   - alfa

   - beta

   - gamma

2. secondo

   - alef

   - bet

   - ghimel

Formattare blocchi di testo
===========================

I blocchi di testo si possono formattare usando il menu a tendina
relativo allo stile negli editor WYSIWYG.

Formattare il codice
--------------------

::

   Questo testo ha lo stile “Source Code”, da usare per gli esempi di codice sorgente

In alternativa, è possibile specificare il linguaggio del codice.

.. code-block:: html

   <a href="#">clicca qui</a>


Citazioni
---------

Questo è un blocco formattato come citazione.

        Frase molto importante di una persona molto famosa.

Paragrafo successivo.

Immagini e tabelle
==================


Immagine (senza didascalia)
---------------------------

|image0|

Figura (con didascalia)
-----------------------

La formattazione centrata non viene resa correttamente in DOCX e ODT. 

.. figure:: media/image1.jpeg
   :width: 2.08403in
   :height: 2.27847in
   :alt: Testo alternativo. Luna
   :align: center
   
   Didascalia della figura, separata dalle opzioni precedenti da una riga vuota. 


Tabella (senza didascalia)
--------------------------

+----+----+----+
| H1 | H2 | H3 |
+----+----+----+
| A1 | A2 | A3 |
+----+----+----+
| B1 | B2 | B3 |
+----+----+----+

Tabella (con didascalia)
------------------------

.. table:: Didascalia della tabella

   +----+----+----+
   | H1 | H2 | H3 |
   +----+----+----+
   | A1 | A2 | A3 |
   +----+----+----+
   | B1 | B2 | B3 |
   +----+----+----+

Note a piè di pagina
====================

Una nota alla fine di una riga [1]_.

- La nota si può mettere anche all'interno di un elenco [2]_.


.. [1] Nota importante.

.. [2] Altra nota importante. 
 
.. |image0| image:: media/image1.jpeg
   :width: 2.08403in
   :height: 2.27847in
   :alt: Testo alternativo. Luna
