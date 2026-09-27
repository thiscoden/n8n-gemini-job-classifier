# KI-gestützte Bewertung von Stellenausschreibungen

Dieses Portfolio-Projekt entwickelt einen selbst gehosteten n8n-Workflow, der
Stellenausschreibungen mit einem konfigurierbaren Kompetenzprofil vergleicht.

## Ziel

Der Workflow soll Stellenausschreibungen strukturiert analysieren, ihre Passung
bewerten und sie für die weitere Bearbeitung in drei Kategorien einteilen:

- A: hohe Passung – Bewerbung priorisieren
- B: teilweise passend – manuell prüfen
- C: geringe Passung – aussortieren

## Geplanter Ablauf

1. Stellenausschreibung einlesen
2. Inhalt bereinigen und normalisieren
3. Duplikate erkennen
4. Anforderungen strukturiert extrahieren
5. Anforderungen mit dem Kompetenzprofil vergleichen
6. Bewertung mit Google Gemini erzeugen
7. Ausgabe gegen ein JSON-Schema validieren
8. Ergebnis speichern und einer Kategorie zuweisen

## Technologien

- Ubuntu Server
- Docker und Docker Compose
- n8n
- PostgreSQL
- Google Gemini API
- Git und GitHub

## Projektstruktur

- `docs/`: Architektur und technische Entscheidungen
- `workflows/`: exportierte n8n-Workflows
- `prompts/`: versionierte KI-Anweisungen
- `schemas/`: strukturierte Ausgabeformate
- `evaluation/`: anonymisierte Evaluationsfälle
- `config/`: ungefährliche Beispielkonfigurationen
- `scripts/`: Backup-, Export- und Testskripte

## Datenschutz

API-Schlüssel, Passwörter, persönliche Lebenslaufdaten, Datenbankinhalte und
Backups werden nicht im Git-Repository gespeichert.

## Status

- [x] Ubuntu-Server analysiert
- [x] Docker Engine und Docker Compose geprüft
- [x] Lokales Git-Repository initialisiert
- [ ] n8n und PostgreSQL konfiguriert
- [ ] HTTPS-Zugriff eingerichtet
- [ ] Gemini-Workflow implementiert
- [ ] Evaluation und Fehlerbehandlung implementiert
- [ ] Backup und Wiederherstellung getestet
