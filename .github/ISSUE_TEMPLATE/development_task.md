---
name: Entwicklungsaufgabe
about: Konkrete Implementierungsaufgabe als Sub-Issue einer User Story oder Technischen Story
title: 'Aufgabe: [Kurzbeschreibung]'
labels: task
assignees: ''
---

<!--
HINWEIS: Eine Entwicklungsaufgabe ist immer ein Sub-Issue — sie gehört zu einer
übergeordneten User Story oder Technischen Story und steht nie allein im Backlog.

WANN wird dieses Template verwendet?
  Im Sprint Planning: Die Aufgaben-Checkliste der übergeordneten Story wird
  finalisiert und jeder Eintrag als Entwicklungsaufgabe angelegt.
  GitHub erlaubt es, Checklisten-Einträge mit einem Klick in verknüpfte Issues
  umzuwandeln — dieses Template füllt das dann entstandene Issue aus.

ZUWEISUNG:
  Jede Entwicklungsaufgabe wird genau einer Person zugewiesen.
  Mehrere Aufgaben derselben Story können parallel von verschiedenen
  Teammitgliedern bearbeitet werden.

Die Story gilt erst als fertig (Done), wenn alle ihre Entwicklungsaufgaben
abgeschlossen sind — unabhängig davon, wer welche Aufgabe bearbeitet hat.
-->

## Übergeordnete Story

**Gehört zu:** #[Issue-Nummer der übergeordneten User Story oder Technischen Story]

<!--
Immer verlinken — eine Entwicklungsaufgabe ohne übergeordnete Story ist nicht zulässig.
-->

---

## Beschreibung

<!--
Was genau ist zu tun? Sei so konkret, dass die Aufgabe ohne Rückfragen
begonnen werden kann. Eine Entwicklungsaufgabe beschreibt genau eine
Aktivität — z. B. einen Endpunkt implementieren, einen Test schreiben,
eine Komponente bauen.
-->

[Präzise Beschreibung der Aufgabe in 1–3 Sätzen.
z. B. „REST-Endpunkt `GET /raeume/verfuegbar` implementieren, der verfügbare Räume
für einen gegebenen Zeitraum zurückgibt. Parameter: `von`, `bis` als ISO-8601-Zeitstempel."]

---

## Fertigstellungskriterium

<!--
Woran erkennt man, dass diese Aufgabe abgeschlossen ist?
Ein konkreter, überprüfbarer Satz genügt — keine lange Liste.
-->

[z. B. „Endpunkt ist implementiert, Unit-Tests sind grün, Code wurde reviewed und gemergt."]

---

## Technische Hinweise

<!--
Optional — aber hilfreich, wenn es relevante Vorgaben, Links oder Fallstricke gibt.
Z. B. Verweis auf ein ADR, eine externe API-Dokumentation oder eine Designvorgabe.
-->

[Technische Details, Links, Hinweise — oder Abschnitt löschen, wenn nicht benötigt]
