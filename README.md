# eclipse-cleaner

## Benutzung
### Vorbereitung
- Abgaben Herunterladen ("Abgaben in Verzeichnissen herunterladen" **muss** aktiviert sein)
- Musterlösung herunterladen
- FileList.txt erstellen oder herunterladen
- **leeres** Ausgabeverzeichnis erstellen
### Programm nutzen
- Programm öffnen und im gui die heruntergeladenen Zip-Verzeichnisse und den Ausgabeordner wählen
- Ausführen drücken
- wenn alles klappt am Besten den log im Ausgabevertzeichnis speichern

### In Eclipse importieren
- Import project->Existing Projects into Workspace
- Dann bei select root directory den Ausgabeordner wählen
-  Viel Spaß beim Korrigieren :D

## Dateiliste Erstellen
Die Dateiliste kann verwendet werden, um Dateien aus der Referenzlösung in alle Abgaben zu kopieren, oder deren Existenz zu prüfen. Dabei müssen alle in der Liste vorkommenden Dateien im Lösungsverzeichnis vorkommen, sonst werden sie ignoriert.
### Modi
- `assert_exists`: Gibt Warnung wenn Datei fehlt (wird **nicht** überschrieben)  
- `assert_not_exists`: Gibt eine Warnung wenn Datei existiert (z.B. sinvoll bei Tutorentests)
- `overwrite_always`: Überschreibt bzw. erstellt Dateien ohne Meldung  
- `copy_if_not_exists`: Kopiert nur wenn Datei noch nicht existiert (keine Meldung)
- `ignore`: ignoriert Dateien (z.B. sinvoll für bin ordner) 
    
Standartmodus Dateiliste: `assert_exists`  
Standartmodus für Dateien die nicht in der Liste Sind: `copy_if_not_exists`
## Bekannte Fehler
- Aktuell macht die Option Abgaben Entpacken noch nichts (ist immer an)

## Mitwirkende
- Kim Berninger (Ersteller)
    - Base Structure
    - Gui
    - Command Line Mode
- Ruben Deisenroth
  - File Extractor
  - Quality of Life improvements
