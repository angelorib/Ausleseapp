# Ausleseapp by Angelo

Web-App zum Auslesen von Zählern über den Bluetooth-IR-Auslesekopf **DvBTIR 7G** (Device GmbH).
Läuft im Browser, braucht keine Installation und keinen Server.

- **Kopf verbinden** – verbindet sich per Bluetooth Low Energy mit dem Auslesekopf
- **Auslesen** – liest den Zähler über die optische Schnittstelle (IEC 62056-21)
- **TXT speichern** – Dateiname ist die Zählernummer
- **Ganzes Objekt auslesen** – mehrere Zähler nacheinander in eine Datei, Dateiname ist die Adresse
- **Experte** – Einstellungen, Protokoll, manuelles Senden

## Voraussetzungen

- Chrome oder Edge (Android, Windows, macOS, Linux)
- iPhone/iPad und Firefox unterstützen Web Bluetooth nicht
- Auslesekopf vorher durch kräftiges Schütteln einschalten

## Auf GitHub Pages veröffentlichen

1. Neues Repository auf GitHub anlegen (z. B. `ausleseapp`).
2. Alle Dateien dieses Ordners hochladen (`index.html`, `manifest.webmanifest`, `sw.js`, Ordner `icons`).
3. Im Repository **Settings → Pages**: Source **Deploy from a branch**, Branch **main**, Ordner **/ (root)**, speichern.
4. Nach etwa einer Minute ist die App erreichbar unter `https://<benutzername>.github.io/ausleseapp/`.

## Auf dem Homebildschirm installieren

1. Link in Chrome auf dem Handy öffnen.
2. Menü (⋮) → **App installieren** bzw. **Zum Startbildschirm hinzufügen**.

## Updates

Wird `index.html` geändert, in `sw.js` die Zeile `const VERSION = 'ausleseapp-v1';` auf eine neue Nummer setzen
(z. B. `ausleseapp-v2`), damit die installierten Apps die neue Version laden.

## Dateien

| Datei | Zweck |
| --- | --- |
| `index.html` | Die App |
| `manifest.webmanifest` | Name, Farben und Symbole für die Installation |
| `sw.js` | Offline-Unterstützung |
| `icons/` | App-Symbole |
