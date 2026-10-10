# BSI Agent Studio

Prototyp: ein Team aus KI-Agenten (Ben D. als Projektmanager, Requirements, Product Owner, Architekt, Entwicklung, QA)
setzt Anforderungen für die BSI Customer Suite um. Ergebnis: ein Export-ZIP.

## Starten (4 Schritte)

1. In VS Code: Menü *Terminal → Neues Terminal*.
2. Prüfen, ob Node da ist: `node -v` (Ergebnis muss mit v22 oder höher beginnen).
3. Starten: `npm start`
4. Im Browser öffnen: http://localhost:8787

Dort oben rechts auf **Live** klicken, als URL `http://localhost:8787/agent-run` eintragen, speichern.
Ohne weitere Einstellung antwortet das Testmodell (Mock): Es beweist den Ablauf, ist aber keine KI.

Beenden: im Terminal `Ctrl+C`.

## Echtes Modell zuschalten

1. Datei `.env.example` kopieren und `.env` nennen.
2. Die drei Zeilen mit `#` entkommentieren und den Schlüssel eintragen.
3. Server stoppen (`Ctrl+C`) und neu starten (`npm start`).

Nur einen von Deloitte freigegebenen Modellzugang verwenden. Den Schlüssel niemals hochladen oder weitergeben.

## Ordner

- `frontend/` die Oberfläche (eine HTML-Datei)
- `backend/` Agenten-Schnittstelle, Modellanbindung, EIP-Generator
- `knowledge/` Wissensordner für Agenten (noch leer)
- `docs/` Demo-Leitfaden und technische Beschreibung

## Status der Export-Artefakte

- EIP-Paket: schema-geprüft (nicht in einer BSI-Instanz importiert)
- Prozess, CX-Design: demo
- „import-validiert" erst nach erfolgreichem Import.
