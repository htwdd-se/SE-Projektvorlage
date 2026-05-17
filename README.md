# Vorlage Projektstruktur & Dokumente

Das Repository enthält die Vorlage einer Projektstruktur und Template-Dokumente
im AsciiDoc-Format. Dies wird für die Bearbeitung der Projektdokumentation in
Software Engineering I und II benötigt. Im Detail sind das:

- Projektstruktur für Code und Dokumente
- Templates der benötigten Dokumente (AsciiDoc-Format)
- Vorlage für die Abgabe in SE I (AsciiDoc-Format)

> [!NOTE]
> Dieses Repository enthält keinen Code.

**Inhaltsverzeichnis**

- [Projektstruktur](#projektstruktur)
- [Dokumentvorlagen](#dokumentvorlagen)
- [Nutzung der AsciiDoc-Vorlagen](#nutzung-der-asciidoc-vorlagen)
- [Repo-Links anpassen](#repo-links-anpassen)
- [Lizenz](#lizenz)

## Projektstruktur

Die Projektstruktur im Verzeichnis **docs** orientiert sich an den wesentlichen
Aspekten im Software Engineering und den für die <ins>Abgabe im SE 1</ins>
geforderten Dokumenten.

```text
docs
├── _includes
│   └── default-attributes.inc.adoc
├── product
│   ├── domains_glossary.adoc
│   └── product_concept.adoc
├── team
│   └── team_charter.adoc
├── technical
│   ├── architecture.adoc
│   ├── design.adoc
│   ├── deployment.adoc
│   └── test_concept.adoc
└── index.adoc
```

## Dokumentvorlagen

Dieses Repository enthält Vorlagen im AsciiDoc-Format zur Dokumentation der
verschiedenen Arbeitsergebnisse.

### Hinweis

Falls Sie Fehler korrigieren oder Verbesserungen machen möchten, können Sie
dies gern über einen _Pull Request_ tun.

## Nutzung der AsciiDoc-Vorlagen

Die Datei _default-attributes.inc.adoc_ im **docs/\_includes** Verzeichnis
enthält die gemeinsamen Dokumentenattribute für alle AsciiDoc-Dokumente. In
jedem Dokument selbst können, nach dem include der Datei, entsprechend noch
zusätzlich benötigte Attribute mit aufgenommen werden.

### Projektname und Systemname definieren

In der _default-attributes.inc.adoc_ Datei ist am Anfang der **Projektname**
und der **Systemname** als Attribute global definiert. Diese können über
`{project-name}` und `{project-system-name}` in der Dokumentation an beliebiger
Stelle verwendet werden.

- **Projektname** `:project-name:`: Enthält das Projektthema inklusive der Projekt-ID
- **Systemname** `:project-system-name:`: Enthält den Systemnamen der Software

```asciidoc
// Meta
:project-name: <Projektname (X0)>
:project-system-name: <Projektname-System>
```

- `X0` ... steht als Platzhalter für die Projekt-ID (bspw. A1, B2)
- `<Platzhalter>` ... die Platzhalter inkl. der `<` und `>` ersetzen

### Bilder und Diagramme einbinden

In dem Dokumentenattribut `:imagesdir: images` ist das Standardverzeichnis
**images** für die Bilder festgelegt. Somit reicht es, in den jeweiligen
Dokumenten, die Bilder ohne Angabe des **images** Verzeichnis einzubinden:

```asciidoc
image::example.jpg[Beispielbild]
```

In dem Dokumentenattribut `:plantumlsdir: plantuml` ist das Standardverzeichnis
**plantuml** für die Diagramme in PlantUML-Notation festgelegt. Im
Dokumentenattribut `:diagramsdir: diagrams` ist das Verzeichnis für die
generierten Diagramme angegeben, welches unter dem `:imagesdir:` angelegt wird.

```asciidoc
product
├── images
│   ├── diagrams
│   │   └── diagram.jpg
│   └── example.jpg
├── plantuml
│   └── diagram.puml
├── ...
└── ux_concept.adoc
```

## Repo-Links anpassen

Bitte ersetzen Sie in den folgenden Dateien `[ORG]/[REPO]` durch den
tatsächlichen Repository-Namen, bevor dieses Projekt produktiv genutzt wird.

- `/.github/ISSUE_TEMPLATE/config.yml`
- `/.github/ISSUE_TEMPLATE/user_story.md`
- `/.github/ISSUE_TEMPLATE/technical_story.md`

## Lizenz

### Dokumentation

Die Templates im Ordner `docs` und `abgabe_se1` unterliegen der
[CC-BY-4.0](https://choosealicense.com/licenses/cc-by-4.0/) Lizenz.

### Quellcode / Anderes

Für das Repository bzw. die entstehende Software muss eine separate Lizenz
festgelegt werden.
