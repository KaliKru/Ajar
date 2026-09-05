# Dotarte — Portfolio-Website

Persönliches Portfolio, live unter **[dotarte.de](https://dotarte.de)**.

## Sichtbarkeit

Die Seite ist **absichtlich nicht in Suchmaschinen auffindbar** — sie ist nur über den direkten Link erreichbar, taucht aber nicht bei Google & Co. auf. Das wird über zwei Dinge sichergestellt:
- `robots.txt` im Hauptverzeichnis (weist Suchmaschinen-Crawler ab)
- `<meta name="robots" content="noindex, nofollow">` im `<head>` jeder Seite

Falls die Seite später doch auffindbar sein soll: beides entfernen.

## Struktur

```
index.html          Hauptseite (Hero, Projekt-Übersicht, Kontakt)
styles.css           Styles der Hauptseite (Creme/Gold/Dunkel, Roboto + Bricolage Grotesque)
robots.txt           Suchmaschinen-Sperre (siehe oben)
images/              Bilder, die nur auf der Hauptseite verwendet werden
projects/
  ajar.html           Case Study „Ajar" (ADHS-Begleiter-App)
  ajar.css            Eigener Stil für die Ajar-Seite (Fraunces/DM Sans, Terrakotta-Akzente)
  images/             Alle Bilder, die zur Ajar-Seite gehören
```

## Tech-Stack

Reines HTML, CSS und Vanilla-JavaScript — keine Frameworks, keine Build-Schritte. Jede Seite ist eine einzelne `.html`-Datei mit eigenem `.css`.

Fonts werden über Google Fonts eingebunden (im `<head>` jeder Seite verlinkt).

## Neues Projekt hinzufügen

1. Neuen Unterordner in `projects/` anlegen (z. B. `projects/seasons/` oder `projects/seasons.html` + `projects/seasons.css` direkt in `projects/`, je nachdem wie viele Bilder das Projekt hat)
2. Auf der Hauptseite (`index.html`) eine der Platzhalter-Karten durch das neue Projekt ersetzen (Bild, Label, Beschreibungstext)
3. Status-Label setzen: `Concept` (goldener Punkt) für laufende Projekte, `Shipped` (grüner Punkt, Klasse `is-shipped`) für abgeschlossene

## Offene Punkte

- **Ajar — Testing & Iteration:** Before/After-Bilder für Runde 3 fehlen noch
- Weitere Projekt-Unterseiten (Seasons, Corporate Identity, Immobilien-Branding) sind auf der Hauptseite als Platzhalter angelegt, eigene Case-Study-Seiten folgen noch
