# Tile-Generator

Dieses Repository enthält ein Python-Skript, welches bestimmte Datenstrukturen (genannt "_tiles") transformiert und modifiziert, basierend auf verschiedenen Input-Parametern.


## Funktionen

- **Color Coding:** Abhängig von der Farbgebung (`color_code`) können Tiles in verschiedenen Farben (z. B. "khaki", "salmon" oder "skyblue") priorisiert und manipuliert werden.
- **Flagging:** Das Skript kann Flags (Kennzeichnungen) hinzufügen oder entfernen, basierend auf den eingegebenen Parametern.
- **Priorität:** Es können Prioritäten gesetzt werden, welche dann in der Reihenfolge ihrer Wichtigkeit verarbeitet werden.
- **Proofreading:** Es gibt eine Option, die ein "Proofreading" (Korrekturlesen) der "_tiles" ermöglicht, um mögliche Fehler zu korrigieren.
- **Farben ändern:** Es gibt eine Option, um die Farben der Tiles zu ändern oder zu behalten (`color_kept`).

## Verwendung

Das Hauptskript verarbeitet Daten wie Temperatur, Farbcodes, Flags und andere Parameter und gibt eine modifizierte Liste von Tiles zurück.  
Diese werden im **JSON-Format** gespeichert, um weiterverarbeitet oder simuliert werden zu können.

## Ausgabeformat

Das Skript generiert oder verändert JSON-Dateien mit folgender Struktur:

```json
{
  "_tiles": [
    {
      "label": "A",
      "glues": [
        { "label": "a", "strength": 1 },
        { "label": "b", "strength": 2 },
        { "label": "c", "strength": 2 },
        { "label": "",  "strength": 0 }
      ],
      "color": "white"
    },
    {
      "label": "B",
      ...
    }
  ]
}
```

## Weiterverwendung in Simulationen

Die erzeugten JSON-Dateien können direkt auf der Website **[NETTAS – Simulator for DNA-based Nanonetworks](https://nettas.itm.uni-luebeck.de/)** hochgeladen werden. Dort können weiter Simulationen auf den Tile-Sets ausgeführt werden.

## Lizenz
Der Quellcode in diesem Repository wird unter der MIT-Lizenz veröffentlicht.
Er darf frei verwendet, verändert und verbreitet werden – auch zu kommerziellen Zwecken – unter der Bedingung, dass die ursprünglichen Urheber genannt werden und keine Haftung übernommen wird.