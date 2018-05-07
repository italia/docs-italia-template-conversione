
#### Confronto della conversione attraverso formati differenti

Usiamo i files in questa cartella per confrontare i risultati
ottenibili con pandoc per convertire da DOCX o da ODT ad RST.

I files `esempio.odt` e `esempio.docx` hanno gli stessi contenuti e
sono stati salvati con libreoffice (versione 5.1). I files
`esempio.odt.rst` ed `esempio.docx.rst` sono stati generati così:

    $ pandoc esempio.odt -o esempio.odt.rst --extract-media ""
    $ pandoc esempio.docx -o esempio.docx.rst --extract-media ""

I risultati sono identici


