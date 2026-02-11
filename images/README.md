# Bilder einfügen - Anleitung

Firma: BRS Malermeister Betrieb

Speichere deine Fotos in diesem Ordner und nutze folgende Dateinamen (klein geschrieben):

## Hero-Sektion (Hintergrundbild)
- Dateiname: `hero-bg.jpg` (optional)
- Aktuelles Beispiel: `dach.jpg`

## Services / Leistungen
- Dateiname-Beispiel: `service-1.jpg` bis `service-4.jpg` (optional)
- Aktuelle Dateinamen im Ordner werden verwendet, wenn vorhanden.

## Referenzen / Projekte
- Dateiname-Beispiel: `project-1.jpg` bis `project-3.jpg` (optional)
- In deinem Ordner sind aktuell: `unnamed.jpg`, `bad.jpg`, `dach.jpg`, `bad schrank.jpg`

## Hinweise
- Formate: JPG oder PNG
- Dateinamen sollten keine Sonderzeichen enthalten (Bsp.: Leerzeichen vermeiden)
- Wenn du eine Datei austauschen willst, ersetze die Datei mit dem gleichen Namen im Ordner.
- Falls du Dateien umbenennen möchtest, nutze diese PowerShell-Befehle (ausgeführt im Projektordner):

```powershell
# Beispiel: rename "bad schrank.jpg" zu "project-2.jpg"
Rename-Item -LiteralPath "images\bad schrank.jpg" -NewName "project-2.jpg"

# Beispiel: kopiere neues Bild in den Ordner
Copy-Item -LiteralPath "C:\Pfad\zu\deinem\neuenbild.jpg" -Destination "images\project-1.jpg"
```

Nach dem Hinzufügen/Umbennen wird die Seite automatisch neu geladen, wenn Live Server aktiv ist.
