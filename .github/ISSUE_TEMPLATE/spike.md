---
name: Spike
about: Zeitlich begrenzte Recherche zur Klärung einer Frage — fachlich oder technisch
title: 'Spike: [Zu untersuchende Frage]'
labels: spike
assignees: ''
---

<!--
HINWEIS: Ein Spike ist eine zeitlich begrenzte Untersuchung, um eine konkrete Frage
zu beantworten und Unsicherheit zu reduzieren. Er endet immer mit einem dokumentierten
Ergebnis — nicht mit einer offenen Diskussion.

Ein Spike ist KEIN:
  - Freies Ausprobieren ohne klares Ziel
  - Ersatz für eine User Story oder Technische Story
  - Endloser Rechercheprozess

Ein Spike wird einer Person oder zwei Personen, die zusammenarbeiten, zugewiesen — nicht dem ganzen Team. Untersuchungen lassen sich nicht sinnvoll parallelisieren.

Zwei Arten von Spikes sind möglich (siehe Feld "Art" unten):

  Produkt-Spike: Reduziert fachliche oder UX-Unsicherheit.
    Beispiele: Nutzerinterviews zur Klärung einer Story; Validierung einer Annahme
    aus dem Produktkonzept; Klärung von Scope oder Priorisierung.
    Ergebnis: Entscheidung, verfeinerte Story, aktualisiertes UX-Konzept oder Persona.

  Technischer Spike: Reduziert technische Unsicherheit.
    Beispiele: Machbarkeit einer API prüfen; zwei Frameworks vergleichen;
    Integrationsproblem untersuchen.
    Ergebnis: ADR, Proof-of-Concept, Empfehlung zwischen Alternativen.
-->

## Art des Spikes

<!--
Genau eine Option auswählen.
-->

- [ ] **Produkt-Spike** — fachliche oder UX-Unsicherheit
- [ ] **Technischer Spike** — technische Unsicherheit

---

## Zu beantwortende Frage

<!--
Formuliere die zentrale Frage als präzisen Fragesatz.
Ein Spike hat genau eine Frage — nicht fünf.
Wenn mehrere Fragen bestehen, mehrere Spikes erstellen.
-->

**Leitfrage:** [z. B. „Welche Informationen brauchen Studierende auf der Raumdetailseite,
bevor wir die Story schreiben?" — oder: „Können wir die Hochschul-LDAP-Schnittstelle
mit Spring Security integrieren, und welche Konfiguration ist nötig?"]

---

## Hintergrund & Motivation

[Warum stellt sich diese Frage? Was wird durch die Antwort ermöglicht oder entsperrt?]

**Blockierte Story / Entscheidung:**
[Link zur blockierten User Story, Technischen Story oder zum offenen ADR — oder „noch offen"]

---

## Time-Box

<!--
Ein Spike hat immer eine feste Zeitgrenze.
Wenn die Zeit abläuft, wird das Ergebnis dokumentiert — auch wenn die Frage
nicht vollständig beantwortet werden konnte. In diesem Fall wird eine Folge-Entscheidung
getroffen: Spike verlängern, anders vorgehen, oder mit Unsicherheit leben.
-->

**Maximale Dauer:** [z. B. 4 Stunden / 1 Tag / 2 Tage]
**Geplant für Sprint:** [Sprint-Nummer oder -Name]
**Bearbeitet von:** [Name oder @mention — Spike wird einer Person oder einem Paar zugewiesen]

---

## Vorgehensweise

<!--
Skizziere kurz den geplanten Ansatz. Das zwingt zur Konkretisierung
und verhindert zielloses Ausprobieren.
-->

- [ ] [z. B. „Vorhandene Nutzerinterviews auf offene Fragen zur Raumdetailseite auswerten"]
- [ ] [z. B. „2 Kurzinterviews mit Studierenden durchführen"]
- [ ] [z. B. „Offizielle Dokumentation der Hochschul-IT lesen"]
- [ ] [z. B. „Minimalen Prototyp mit Spring Boot + LDAP aufbauen"]
- [ ] [Weiterer Schritt]

---

## Erwartetes Ergebnis

<!--
Was soll am Ende des Spikes vorliegen?
Das Ergebnis ist immer ein konkretes Artefakt — kein „wir haben darüber geredet".
-->

- [ ] Klare Antwort auf die Leitfrage (dokumentiert im Abschnitt „Ergebnis" unten)
- [ ] Empfehlung oder Entscheidung für das weitere Vorgehen
- [ ] [z. B. „ADR in `architecture.adoc` erstellt" — bei technischem Spike]
- [ ] [z. B. „UX-Konzept oder Persona aktualisiert" — bei Produkt-Spike]
- [ ] [z. B. „Proof-of-Concept-Code in Branch `spike/ldap` verfügbar"]
- [ ] Folgeaufgaben als neue Issues erstellt (User Stories, Technische Stories oder Bugs)

---

## Ergebnis

<!--
Dieser Abschnitt wird NACH Abschluss des Spikes ausgefüllt — vor dem Schließen des Issues.
Ein Spike ohne dokumentiertes Ergebnis gilt nicht als abgeschlossen.
-->

**Antwort auf die Leitfrage:**
[Nach Abschluss ausfüllen]

**Empfehlung / Entscheidung:**
[Nach Abschluss ausfüllen]

**Folgeaufgaben:**
[Links zu Issues, ADRs oder Dokumenten, die aus diesem Spike entstanden sind]
