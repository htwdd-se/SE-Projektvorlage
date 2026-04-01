---
name: Technische Story
about: Technische Arbeit mit eigenem fachlichen Wert, die nicht direkt aus einer User Story abgeleitet ist
title: 'Tech-Story: [Kurzbeschreibung]'
labels: technical-story
assignees: ''
---

<!--
HINWEIS: Eine Technische Story ist ein vollwertiges Product Backlog Item — kein
Sub-Issue einer User Story. Sie beschreibt technische Arbeit, die einen eigenständigen
Wert für das Projekt hat: Infrastruktur aufbauen, technische Schulden abbauen,
Sicherheit verbessern, Dokumentation erstellen.

Der Unterschied zu einer Entwicklungsaufgabe (Sub-Issue):
  Technische Story: steht eigenständig im Backlog; hat eigene Begründung und DoD
  Entwicklungsaufgabe: ist ein Sub-Issue einer User Story oder Technischen Story

Typische Anwendungsfälle:
  - CI/CD-Pipeline aufbauen
  - Datenbankmigrationen einführen (Flyway / Liquibase)
  - Technische Schulden abbauen (Refactoring, veraltete Abhängigkeiten)
  - Sicherheitslücken beseitigen
  - Performance-Engpässe beheben
  - Projektdokumentation erstellen oder aktualisieren

ABLAUF:
  Refinement: Beschreibung + Akzeptanzkriterien ausfüllen; Aufgaben-Checkliste skizzieren
  Planning: Checkliste finalisieren; Einträge als Sub-Issues anlegen und zuweisen
-->

## Beschreibung

[Was soll gemacht werden? Beschreibe die Aufgabe klar und konkret in 2–4 Sätzen.]

---

## Begründung

<!--
Warum ist diese Story notwendig?
Welches Problem löst sie, oder welchen Nutzen bringt sie dem Projekt?
Eine Technische Story ohne Begründung ist nicht priorisierbar.
-->

[Warum wird diese Arbeit gebraucht? Welchen Nutzen hat sie für das Team, das Produkt
oder die Qualität? — Verweis auf ein Qualitätsziel oder eine Einschränkung aus dem
Produktkonzept, falls zutreffend.]

---

## Bezug zu anderen Artefakten

**Zugehöriges ADR:**
[Link zum ADR in `architecture.adoc` — oder „nicht zutreffend"]

**Betroffene User Stories:**
[Links zu Stories, die diese Arbeit voraussetzen oder davon profitieren — oder „keine"]

**Dokumentation betroffen:**
[Welche Dokumente in `/docs` müssen ebenfalls aktualisiert werden? — oder „keine"]

---

## Akzeptanzkriterien

<!--
Wie bei User Stories: konkret und testbar.
Für technische Arbeit sind oft einfache testbare Aussagen passender als das Given/When/Then-Format.
Mindestens 2 Kriterien.
-->

- [ ] [z. B. „CI-Pipeline ist grün bei jedem Push auf main."]
- [ ] [z. B. „Alle bestehenden Tests bestehen nach dem Refactoring."]
- [ ] [z. B. „Technische Änderung ist in `architecture.adoc` oder `design.adoc` dokumentiert."]
- [ ] [Weiteres Kriterium]

---

## Aufgaben-Checkliste

<!--
REFINEMENT: Gemeinsam vom Team erarbeitet — welche Entwicklungsaufgaben sind ötig?
PLANNING: Einträge als Sub-Issues anlegen und zuweisen.
-->

- [ ] [z. B. Pipeline-Konfiguration schreiben (`.github/workflows/ci.yml`)]
- [ ] [z. B. Secrets in GitHub Repository konfigurieren]
- [ ] [z. B. Deployment auf Staging-Umgebung testen]
- [ ] [z. B. `deployment.adoc` aktualisieren]
- [ ] [Weiterer Schritt]

---

> **Definition of Ready** prüfen, bevor diese Story in einen Sprint aufgenommen wird:
> [Team-Charta - Definition of Ready](https://github.com/[ORG]/[REPO]/blob/main/docs/team/team_charter.adoc)
