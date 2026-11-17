# Talglück 3D – Aufbauspiel (V10)

Ein friedliches Aufbauspiel für Kinder und Erwachsene – ganz ohne Krieg.
Baue Wege, Häuser und Warenketten, entdecke mit der Forscherin Tiere, Steine und Sterne,
rette gestrandete Meerestiere und schalte neue Gebiete frei.

Läuft im Browser auf **Android, iPhone/iPad und PC** und lässt sich als App installieren (PWA).
Nach dem ersten Laden funktioniert das Spiel auch **offline**.

## Dateien

| Datei | Zweck |
|---|---|
| `index.html` | Das komplette Spiel (eine Datei, alle Grafiken und Modelle eingebettet) |
| `manifest.webmanifest` | App-Beschreibung für die Installation (Name, Farben, Symbole) |
| `sw.js` | Service Worker – speichert das Spiel für die Offline-Nutzung |
| `icons/` | App-Symbole (192 px, 512 px, „maskable“ für Android, Apple-Touch-Icon, Favicon) |
| `.nojekyll` | Sorgt dafür, dass GitHub Pages alle Dateien unverändert ausliefert |

## Auf GitHub veröffentlichen (GitHub Pages)

1. Neues Repository anlegen, z. B. `talglueck-3d`.
2. **Den Inhalt dieses Ordners** hochladen (nicht den Ordner selbst): *Add file → Upload files*,
   alle Dateien und den Ordner `icons` hineinziehen, dann *Commit changes*.
3. *Settings → Pages* → Source: **Deploy from a branch** → Branch **main**, Ordner **/ (root)** → *Save*.
4. Nach ein bis zwei Minuten ist das Spiel erreichbar unter
   `https://<dein-github-name>.github.io/talglueck-3d/`

## Als App installieren

- **Android (Chrome):** Seite öffnen → Menü ⋮ → *App installieren* bzw. *Zum Startbildschirm hinzufügen*.
- **iPhone/iPad (Safari):** Seite öffnen → Teilen-Symbol → *Zum Home-Bildschirm*.
- **PC (Chrome/Edge):** Installationssymbol rechts in der Adressleiste.

## Neue Version hochladen

1. Neue `index.html` hochladen (ersetzen).
2. In `sw.js` die Zeile `const CACHE = 'talglueck-3d-v10';` auf die neue Nummer ändern (z. B. `v11`)
   und mit hochladen – dann holen sich installierte Apps die neue Version automatisch.
3. In dieser README die Versionsnummer anpassen.

## Spielstände

Die 10 Speicherplätze und die Bücher werden **im Browser des jeweiligen Geräts** gespeichert.
Sie gehören zur Web-Adresse: Spielstände aus der Claude-Vorschau oder einer anderen Adresse
erscheinen auf GitHub Pages nicht automatisch – dafür im Spiel *Menü → Spielstand exportieren*
und auf der neuen Seite *importieren*.

## Version

**V10** – neue Baumarten (Ahorn, Säulenbirke, Säulenbaum), Gebiete mit eigenen Regeln,
Schlittschuhlaufen, Sternwarte, Meer, Vulkan, Forscher-Bücher u. v. m.

Verwendete Bibliothek: three.js (MIT-Lizenz). 3D-Modelle für Marktstände und Karren: Kenney (CC0).
