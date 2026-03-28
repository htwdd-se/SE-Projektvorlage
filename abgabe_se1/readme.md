# Abgabe in SE I

Im Verzeichnis **abgabe_se1** finden Sie die Vorlagedatei
_se1_projektdokumentation_x0.adoc_, welche alle Ihre erzeugten Dokumente für die Abgabe als
PDF in <ins>ein</ins> Dokument bündelt.

Folgende Schritte sind für eine Abgabe durchzuführen:

1. Ändern Sie die Projek-ID **x0** in der Vorlagedatei
   _se1_projektdokumentation_x0.adoc_ in Ihre Themennummer (a1, a2, b1, ...).
2. Inhalt der Vorlagedatei anpassen:
   - Ist in Ihrem Projekt in der Datei
     _docs/\_includes/default-attributes.inc.adoc_ der Projektname im Attribut
     `:project-name:` nicht gesetzt bzw. nutzen Sie eine andere Struktur,
     können Sie im Dokumententitel nach dem `:` das `{project-name}` mit Ihrem
     Projektthema ersetzen:

     ```asciidoc
     // --- 1. Projektthema -------------------------
     = SE I - Projektdokumentation: {project-name}
     ```

   - Tragen Sie **alle** Teammitglieder als Autoren ein:

     ```asciidoc
     // --- 2. Teammitglieder -----------------------
     Vorname Nachname <s00000@htw-dresden.de>; Vorname Nachname <s00000@htw-dresden.de>; ...
     ```

     > Lange Autorennamen (mehr als 3 Teile) in den Dokumentenattributen müssen
     > mit einem `_` (Unterstrich) zu einer Gruppe von Vor- bzw. Nachnamen
     > zusammengefasst werden. Es treten sonst Formatierungsfehler beim
     > erzeugen der HTML- oder PDF-Dokumente auf. Der `_` (Unterstrich) wird im
     > erzeugten Dokument nicht dargestellt.
     >
     > - `Vorname1_Vorname2 Nachname1_Nachname2 <mail@example.com>`
     > - `Vorname Nachname1_Nachname2_Nachname3 <mail@example.com>`

   - Tragen Sie als Versionsdatum Ihr **Abgabedatum** ein:

     ```asciidoc
     // --- 3. Abgabedatum --------------------------
     01. Januar 2020
     ```

   - Passen Sie bei abweichender Projektstruktur die **include-Pfade** und
     **Dateinamen** zu den einzelnen Dateien (_path/to/file.adoc_) an bzw.
     erweitern Sie es für zusätzliche Dokumente:

     ```asciidoc
     include::path/to/file.adoc[lines=1..1;4..-1,leveloffset=+1]
     ```

     > Beim `include` wird über die `lines=1..1;4..-1` Angabe jeweils die 1.
     > und alles ab der 4. Zeile übernommen. Jedes Dokument ist eigenständig
     > und somit werden über die Zeilen 2 und 3 die jeweiligen Autoren und das
     > Versionsdatum nicht mit übernommen.

3. Erzeugen Sie das Abgabe-PDF _*se1_projektdokumentation_x0.pdf*_ ([Hinweise aus dem
   Praktikum](https://www.informatik.htw-dresden.de/~zirkelba/praktika/se/git-docs-collab/01-basics.html#_htmlpdf_generierung)):

   ```sh
   asciidoctor-pdf se1_projektdokumentation_x0.adoc
   ```

   ```sh
   # mit PlantUML
   asciidoctor-pdf -r asciidoctor-diagram se1_projektdokumentation_x0.adoc
   ```

   oder:

   ```sh
   asciidoctor -r asciidoctor-pdf -b pdf se1_projektdokumentation_x0.adoc
   ```

   ```sh
   # mit PlantUML
   asciidoctor -r asciidoctor-diagram -r asciidoctor-pdf -b pdf se1_projektdokumentation_x0.adoc
   ```

4. Prüfen Sie, dass das korrekte **Projektthema**, alle **Teammitglieder** und
   das **Abgabedatum** auf dem Deckblatt stehen und dass ebenfalls alle
   erforderlichen **Dokumente** mit ihren Inhalten enthalten sind.

5. Geben Sie das finale Abgabe-PDF _*se1_projektdokumentation_x0.pdf*_ über den
   mitgeteilten Weg ab.
