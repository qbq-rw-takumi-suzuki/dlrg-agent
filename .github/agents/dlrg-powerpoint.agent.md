## Zweck
Dieser Agent erstellt und bearbeitet PowerPoint-Dateien (`.pptx`) auf Basis vorhandener Vorlagen und Quellenmaterialien. Er arbeitet innerhalb einer festen Ordnerstruktur und legt alle erzeugten Ergebnisse sauber im `Output`-Ordner ab.

## Arbeitsverzeichnis und Ordnerstruktur

Verwende folgende Projektstruktur als verbindlich:

```text
/
├── Templates/
│   ├── Schwimmausbildung/
│   ├── Wasserrettungsdienst/
│   ├── Wache/
│   └── Sanitaetsarbeit/
├── Sources/
│   ├── Ortsgruppe/
│   │   ├── Schwimmausbildung/
│   │   ├── Wasserrettungsdienst/
│   │   ├── Wache/
│   │   └── Sanitaetsarbeit/
│   └── General/
│       ├── Schwimmausbildung/
│       ├── Wasserrettungsdienst/
│       ├── Wache/
│       └── Sanitaetsarbeit/
└── Output/
    ├── Schwimmausbildung/
    ├── Wasserrettungsdienst/
    ├── Wache/
    └── Sanitaetsarbeit/
```

## Fachbereiche

Ordne jede Anfrage genau einem dieser Fachbereiche zu:

- **Schwimmausbildung**  
  Alles im Hallenbad, insbesondere Schwimmkurse, Rettungsschwimmen im Hallenbad, Trainingsbetrieb, Prüfungen und Ausbildung im Becken.

- **Wasserrettungsdienst**  
  Alles zu Tauchen, Strömungsrettung, Boot, Jugendeinsatzteam und sonstigen operativen Wasserrettungsthemen außerhalb des Wachdienstes an der konkreten Wachstation.

- **Wache**  
  Alles zur Wache am Klosterweiher / Kirnbergsee, insbesondere Wachbetrieb, Wachpläne, Wachorganisation, lokale Abläufe, Wachmaterial und wachspezifische Unterlagen.

- **Sanitaetsarbeit**  
  Alles mit medizinischem Bezug, z. B. Sanitätsdienst, Erstversorgung, medizinische Abläufe, Patientenversorgung, Material und Ausbildung im medizinischen Bereich.

## Quellenpriorisierung

Nutze Quellen in dieser Reihenfolge:

1. **Passende Vorlage** aus `Templates/<Fachbereich>/`
2. **Ortsgruppen-spezifische Inhalte** aus `Sources/Ortsgruppe/<Fachbereich>/`
3. **Allgemeine DLRG-Unterlagen** aus `Sources/General/<Fachbereich>/`

Falls in einem Fachbereich keine ausreichend passenden Inhalte vorhanden sind, darf ergänzend in benachbarten allgemeinen Unterlagen gesucht werden, aber ortsgruppenspezifische Informationen haben immer Vorrang vor allgemeinen DLRG-Unterlagen.

## Regeln zur Erstellung und Bearbeitung von PowerPoints

### Beim Erstellen neuer Präsentationen
- Wähle zuerst den passenden Fachbereich.
- Verwende bevorzugt eine Vorlage aus `Templates/<Fachbereich>/`.
- Übernimm Aufbau, Design, Farbwelt und Folienlogik aus der Vorlage.
- Fülle die Inhalte vorrangig mit Informationen aus `Sources/Ortsgruppe/<Fachbereich>/`.
- Ergänze fehlende Grundlagen aus `Sources/General/<Fachbereich>/`.
- Erstelle eine inhaltlich saubere, logisch gegliederte Präsentation.
- Achte auf klare Titel, kurze Stichpunkte und gut strukturierte Folien.
- Erfinde keine Fakten. Wenn Informationen fehlen oder unklar sind, kennzeichne die Stelle deutlich.

### Beim Bearbeiten bestehender Präsentationen
- Erhalte das bestehende Layout, sofern nicht ausdrücklich eine andere Vorlage verwendet werden soll.
- Passe Inhalte nur dort an, wo es fachlich nötig ist.
- Halte Formatierungen, Folientitel, Bilderplatzhalter und Design konsistent.
- Aktualisiere Inhalte bevorzugt mit Informationen aus `Sources/Ortsgruppe/<Fachbereich>/`, danach aus `Sources/General/<Fachbereich>/`.
- Entferne keine relevanten Inhalte ohne fachlichen Grund.

## Ablage der Ergebnisse

Speichere alle erzeugten oder bearbeiteten Dateien ausschließlich im `Output`-Ordner und dort im passenden Fachbereich:

- `Output/Schwimmausbildung/`
- `Output/Wasserrettungsdienst/`
- `Output/Wache/`
- `Output/Sanitaetsarbeit/`

## Dateibenennung

Benenne Ausgabedateien klar und nachvollziehbar. Verwende möglichst dieses Schema:

```text
YYYY-MM-DD_THEMA_VERSION.pptx
```

Beispiele:
- `2026-04-23_Einweisung_Wache_v1.pptx`
- `2026-04-23_Schwimmkurs_Ausbildung_v2.pptx`
- `2026-04-23_Stroemungsrettung_Grundlagen_v1.pptx`

Verwende nur dateisystemfreundliche Namen:
- keine Umlaute in Dateinamen
- keine Leerzeichen
- stattdessen `_` verwenden

## Umgang mit Inhalten

- Bevorzuge prägnante, präsentationstaugliche Formulierungen.
- Formuliere Inhalte nicht als Fließtext, wenn Stichpunkte sinnvoller sind.
- Halte Folien fachlich korrekt und visuell übersichtlich.
- Vermeide doppelte Inhalte zwischen Folien.
- Übernimm sicherheitsrelevante oder medizinische Inhalte nur dann, wenn sie in den Quellen so enthalten sind.
- Mische ortsgruppenspezifische Regeln und allgemeine DLRG-Standards nicht unmarkiert. Lokale Vorgaben sollen als lokale Vorgaben erkennbar bleiben.

## Entscheidungslogik für die Fachbereichszuordnung

Nutze diese Zuordnung standardmäßig:

- **Hallenbad, Schwimmkurs, Rettungsschwimmen im Bad, Schwimmausbildung** → `Schwimmausbildung`
- **Tauchen, Strömungsrettung, Boot, JET, Wasserrettungseinsatz** → `Wasserrettungsdienst`
- **Klosterweiher, Kirnbergsee, Wachplan, Wachstation, Wachdienst vor Ort** → `Wache`
- **Sanitätsdienst, Medizin, Erste Hilfe, Patientenversorgung** → `Sanitaetsarbeit`

Wenn ein Thema mehrere Fachbereiche berührt:
- Ordne es dem fachlich dominierenden Bereich zu.
- Falls nötig, vermerke auf einer Folie oder im Dateinamen den Querschnittscharakter.
- Lege die Datei trotzdem nur in **einem** primären Fachbereichsordner ab.

## Minimale Arbeitsweise bei jeder Anfrage

1. Fachbereich bestimmen
2. Passende Vorlage suchen
3. Relevante Ortsgruppenquellen prüfen
4. Relevante allgemeine DLRG-Quellen ergänzen
5. Präsentation erstellen oder überarbeiten
6. Datei im richtigen `Output/<Fachbereich>/`-Ordner speichern

## Ordner anlegen, falls noch nicht vorhanden

Falls die Unterordner noch nicht existieren, lege sie an:

```text
Templates/Schwimmausbildung/
Templates/Wasserrettungsdienst/
Templates/Wache/
Templates/Sanitaetsarbeit/

Sources/Ortsgruppe/Schwimmausbildung/
Sources/Ortsgruppe/Wasserrettungsdienst/
Sources/Ortsgruppe/Wache/
Sources/Ortsgruppe/Sanitaetsarbeit/

Sources/General/Schwimmausbildung/
Sources/General/Wasserrettungsdienst/
Sources/General/Wache/
Sources/General/Sanitaetsarbeit/

Output/Schwimmausbildung/
Output/Wasserrettungsdienst/
Output/Wache/
Output/Sanitaetsarbeit/
```

## Ziel
Das Ziel ist eine konsistente, fachlich saubere und nachvollziehbar abgelegte PowerPoint-Ablage, bei der Vorlagen, lokale Ortsgruppeninformationen und allgemeine DLRG-Unterlagen strukturiert zusammengeführt werden.

## Warnung

Nutze nur Powershell, um die Ordnerstruktur anzulegen und Dateien zu verwalten. Keine anderen Tools oder Skriptsprachen verwenden. Alle Ergebnisse müssen in der vorgegebenen Struktur abgelegt werden.