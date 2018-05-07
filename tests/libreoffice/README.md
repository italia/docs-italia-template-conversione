
#### Confronto della conversione attraverso formati differenti

Usiamo i files in questa cartella per confrontare i risultati
ottenibili con pandoc per convertire da DOCX o da ODT ad RST.

I files `esempio.odt` e `esempio.docx` hanno gli stessi contenuti e
sono stati salvati con libreoffice (versione 5.1). I files
`esempio.odt.rst` ed `esempio.docx.rst` sono stati generati così:

    $ pandoc esempio.odt -o esempio.odt.rst --extract-media ""
    $ pandoc esempio.docx -o esempio.docx.rst --extract-media ""

#### Risultato

```
 libreoffice (master)*$ diff esempio.*.rst
43,45c43,44
< ::
< 
<    Questo testo ha lo stile “Source Code”, da usare per gli esempi di codice sorgente
---
> Questo testo ha lo stile “Source Code”, da usare per gli esempi di
> codice sorgente
55,56d53
< |image0|
< 
61,62d57
< | H1 | H2 | H3 |
< +----+----+----+
76,78c71
< .. |image0| image:: /media/image1.jpeg
<    :width: 2.08403in
<    :height: 2.27847in
---
> 
```

Il file convertito da ODT presenta diversi problemi: il codice non è
formattato come tale, gli headers della tabella non vengono mostrati e
l'immagine viene omessa del tutto.

