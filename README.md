# Portfolio Website

Die Seite besteht jetzt aus drei Teilen:
- `index.html` — die Struktur/Inhalte
- `styles.css` — alle Styles
- `images/` — die Bilddateien (5 PNGs)

## Veröffentlichen mit GitHub Pages

1. **Neues Repository erstellen**
   - Auf [github.com](https://github.com) einloggen → oben rechts auf **+** → **New repository**
   - Name z. B. `portfolio` (der Name wird Teil der URL, außer du nutzt ein "User Page"-Repo, siehe unten)
   - Öffentlich (**Public**) auswählen
   - "Add a README" NICHT anhaken (wir laden unsere eigene hoch)
   - **Create repository**

2. **Dateien hochladen**
   - Im neuen Repo auf **Add file → Upload files**
   - **Wichtig:** Zieh den kompletten Ordnerinhalt (also `index.html`, `styles.css`, `README.md` UND den ganzen `images`-Ordner mit den 5 PNGs darin) auf einmal per Drag & Drop in das Upload-Fenster. GitHub erhält dabei die Ordnerstruktur (`images/...`) automatisch.
   - Falls Drag & Drop des Ordners nicht klappt: Erstelle im Repo zuerst manuell einen Ordner namens `images` (z. B. über "Create new file" → `images/.gitkeep` → committen), öffne ihn, und lade die 5 PNGs dort einzeln hoch.
   - Unten **Commit changes** klicken

3. **GitHub Pages aktivieren**
   - Im Repo auf **Settings** (oben in der Repo-Navigation)
   - Im linken Menü auf **Pages**
   - Unter **Source** → **Deploy from a branch** wählen
   - Branch: `main`, Ordner: `/ (root)` → **Save**

4. **Fertig**
   - Nach ca. 1–2 Minuten ist die Seite live unter:
     `https://DEIN-BENUTZERNAME.github.io/REPO-NAME/`
   - Die URL steht auch oben im Pages-Einstellungsbereich, sobald das Deployment durchgelaufen ist (grünes Häkchen)

## Eigene Domain (optional)

Falls du später eine eigene Domain verbinden willst (z. B. `deinname.de`):
- Im Pages-Bereich unter **Custom domain** die Domain eintragen
- Bei deinem Domain-Anbieter einen `CNAME`-Eintrag auf `DEIN-BENUTZERNAME.github.io` setzen (Details dazu liefert GitHub direkt im Pages-Bereich)

## Änderungen später vornehmen

Jede Änderung an `index.html`, `styles.css` oder einem Bild im Repo (z. B. über **Edit** direkt auf GitHub oder erneutes Hochladen) wird automatisch neu deployed — meist innerhalb von 1–2 Minuten sichtbar.

## Bilder später ersetzen

Wenn du bessere Exports der App-Screens hast: einfach die entsprechende Datei im `images`-Ordner mit gleichem Dateinamen überschreiben (z. B. `phone3-detail.png` erneut hochladen und beim Hochladen bestätigen, dass die alte Version ersetzt wird). Die `index.html` muss dafür nicht angepasst werden, solange der Dateiname gleich bleibt.
