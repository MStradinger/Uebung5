# Übung 05 – Webdev Toolchain

Die Testseite zeigt ein responsives Bootstrap-Raster, mehrere Button-Varianten und Bootstrap-Icons. Sass lädt die benötigten Bootstrap-Module mit `@use`. Das Projekt verwendet dafür Bootstrap 6.0.0-alpha.1.

## Voraussetzungen

- Node.js ab Version 20.19.0 mit npm
- Git

## Installation

1. Kopiere auf GitHub die HTTPS-URL des Repositories unter **Code** und setze sie anstelle der Beispiel-URL ein.

   ```sh
   git clone https://github.com/DEIN-NAME/bootstrap-projekt.git bootstrap-projekt
   cd bootstrap-projekt
   ```

2. Installiere die Abhängigkeiten und kompiliere das Stylesheet.

   ```sh
   npm install
   npm run scss:build
   ```

## Lokale Entwicklung

Starte diese Befehle in zwei Terminals im Projektordner.

| Befehl | Funktion |
| --- | --- |
| `npm run scss:watch` | Kompiliert Änderungen an `src/scss/style.scss` automatisch nach `dist/css/style.css`. |
| `npm run serve` | Startet BrowserSync und aktualisiert die Seite bei Änderungen an HTML oder CSS. |

Öffne die von BrowserSync angezeigte lokale URL. Ändere zum Testen einen Text in `index.html` oder die Primärfarbe `$primary` in `src/scss/style.scss` und speichere die Datei. Die Änderung sollte direkt im Browser sichtbar sein. Mit `Strg+C` beendest du die beiden Befehle.

`npm run scss:build` erzeugt das CSS einmalig. Git ignoriert den Ordner `dist/`, da der Build seinen Inhalt aus dem Quellcode erzeugt.
