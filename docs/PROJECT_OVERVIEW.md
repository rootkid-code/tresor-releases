# Tresor Beta Lab · Release- und Dokumentationsleitfaden

> [!CAUTION]
> **Ausnahmslos Beta-Testsoftware.** Keine echten Dateien, persönlichen Daten, Passwörter, vertraulichen Dokumente oder unersetzlichen Inhalte mit Tresor speichern. Nur künstliche, austauschbare Testdaten verwenden.

## Rolle dieses Repositories

Dieses **öffentliche Repository** ist die Distributions- und Dokumentationsfläche für experimentelle Windows-Testpakete. Die private Entwicklung findet separat in [`rootkid-code/tresor`](https://github.com/rootkid-code/tresor) statt. Keine Veröffentlichung ist als Produktivfreigabe zu verstehen.

## Informationsarchitektur

| Bereich | Zweck |
| --- | --- |
| [`README.md`](../README.md) | Deutsche Hauptansicht mit Originalgrafiken, Sicherheitswarnung, Entwicklungsstand und Roadmap |
| [`README.en.md`](README.en.md) | Vollständige englische Fassung |
| [`assets/`](../assets/) | Eigene deutsche und englische SVG-Konzeptillustrationen; **keine Screenshots** |
| [GitHub Releases](https://github.com/rootkid-code/tresor-releases/releases) | Tatsächlich veröffentlichte Beta-Testpakete und gegebenenfalls zugehörige Prüfsummen |
| [Dieses Dokument](PROJECT_OVERVIEW.md) | Verantwortung, Status und Qualitätssicherung der Distribution |

## Veröffentlichungsstatus

Stand der Dokumentationskontrolle: **21. November 2026**.

- Zuletzt bestätigte öffentliche Beta: `v0.1.1-beta.12`.
- `v0.1.1-beta.13` ist im privaten Quellprojekt vorbereitet, aber nicht als öffentliches Release bestätigt.
- Keine stabile Version und keine Sicherheits- oder Produktivfreigabe.

## Gestaltung

Die Visualisierung soll professionell erklären, **was das Projekt untersucht und was es ausdrücklich nicht leistet**. Daher werden Konzeptgrafiken als solche gekennzeichnet. Es werden keine fiktiven Testergebnisse, Siegel, Kundenlogos oder Sicherheitszertifikate dargestellt.

## Vor einer künftigen Freigabe notwendig

Unabhängige Sicherheitsprüfung, externe Anti-Rollback-Sicherung, echte Restore-/Migrations-/Ausfalltests, Windows-Geräte- und Updateprüfungen, überprüfbare Release-Signaturen und dokumentierte Akzeptanzkriterien. Die Einzelheiten stehen in beiden Sprachversionen.

## Prüfkriterien für README-Änderungen

- Warnung vor Echt-Daten bleibt vor Funktionen/Downloadangebot.
- Deutsche und englische Fassung bleiben inhaltlich konsistent.
- Release-Aussagen werden anhand tatsächlich veröffentlichter Assets geprüft.
- Illustrationen werden nie als Produkt-Screenshots ausgegeben.
- Keine Secrets, Kundendaten oder Signaturschlüssel in Markdown, SVG oder Git-Historie aufnehmen.

*Ein ausführliches Erscheinungsbild ist keine Aussage über die Einsatzreife.*
