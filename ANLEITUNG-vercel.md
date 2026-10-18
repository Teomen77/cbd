# ciya bakir design – Website aktualisieren (Vercel)

Dieser Ordner ist die komplette Website. Es gibt keinen Build-Schritt und keine Datenbank: Vercel liefert die Dateien einfach so aus.

## Inhalt
- `index.html` – Startseite (alles drin: Styles, Schrift, Skripte)
- `impressum.html`, `datenschutz.html` – Unterseiten (werden auch als Fenster auf der Startseite geöffnet, deshalb müssen beide Inhalte gleich bleiben, wenn du etwas änderst)
- `brand/` – Logos, Favicon, Vorschaubild (og.png)
- `robots.txt`, `sitemap.xml`, `llms.txt` – für Suchmaschinen und KI-Assistenten

## Texte ändern
Alles Sichtbare steht in `index.html`. Suchen (Strg+F / Cmd+F) nach dem Satz, den du ändern willst, und ersetzen. Die Wörter, die im Footer wechseln, stehen in der Liste `<ul>` unter `<footer>`.

Wichtig: Impressum und Datenschutz stehen sowohl in der jeweiligen `.html`-Datei als auch als Fenster in `index.html`. Ändert man eins, am besten das andere auch.

Das Impressum enthält den Hinweis zur Kleinunternehmerregelung (§ 19 UStG) und keine Umsatzsteuer-ID. Sollte Ciya später eine USt-IdNr. bekommen, muss sie dort ergänzt werden (§ 27a UStG).

## Veröffentlichen mit Vercel (einmalig)
1. Projekt auf vercel.com anlegen: „Add New … → Project“ → „Import” oder den Ordner per Drag & Drop in das Dashboard ziehen (Framework: „Other“, kein Build-Befehl, Output-Verzeichnis leer lassen).
2. Nach dem Deployment bekommst du eine Vorschau-URL. Die kannst du prüfen, bevor etwas live geht.
3. Domain hinzufügen: Projekt → Settings → Domains → `www.ciyabakirdesign.com` eintragen. Vercel zeigt dir dann, welche DNS-Einträge beim Domain-Anbieter gesetzt werden müssen (meist ein CNAME für `www` und ein A-Record für die Root-Domain `76.76.21.21`). Das muss in den DNS-Einstellungen der Domain gemacht werden, nicht bei Vercel.

## Aktualisieren
Einfach die geänderten Dateien ersetzen und neu hochladen (Drag & Drop auf das Projekt) oder – wenn das Projekt mit GitHub verbunden ist – committen und pushen. Vercel veröffentlicht automatisch.

## Zurück zur alten Version (Rollback)
Im Vercel-Projekt unter „Deployments“ die vorherige Version auswählen → „…“ → „Promote to Production“ bzw. „Instant Rollback“. Das dauert Sekunden und betrifft nur die Ansicht, nichts wird gelöscht.

Vorher einmal sichern: Die alte Seite (die passwortgeschützte Version) ist nicht in diesem Ordner. Falls sie noch irgendwo liegt, bitte vor dem Umschalten herunterladen.

## Kontakt
c@ciyabakirdesign.com
