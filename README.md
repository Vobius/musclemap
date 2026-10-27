# MuscleMap

Interactive muscle map for building workout plans. Click muscles on an anatomical SVG, and get matching exercises with their primary and secondary muscle targets.
> 🇩🇪 The MuscleMap UI is entirely in **German** (muscle and exercise names), with Latin muscle terms alongside.

Everything lives in **one single HTML file**. No build step, no dependencies, no server. Just open it in your browser.

## Features

- Anatomical SVG with clickable muscle groups
- Exercise database (35 exercises) with primary and secondary target muscles
- Muscle names in German and Latin
- Works fully offline
- Lightweight: one small file, loads instantly

## Usage

1. Download `form-muskelkarte(4).html`
2. Open it in any modern browser
3. Click the muscles you want to train and see the matching exercises

## Customizing

Exercises are stored as a simple JS array inside the file:

```js
{
  "name": "Reverse Butterfly",
  "category": "Isolationsübungen",
  "group": "ruecken",
  "primary": ["deltoid_hinten"],
  "secondary": ["trapez_mitte_rhomboiden", "trapez_oben"]
}
```

- `primary` / `secondary` use the muscle IDs from the SVG (`data-muscle` attribute)
- To add an exercise, add a new entry to the array
- Make sure every muscle ID you use also exists in the SVG

## Tech

- Plain HTML, CSS and JavaScript
- Inline SVG
- No frameworks, no external requests

## License

not yet

## Author

Lu Vobius

# MuscleMap

Interaktive Muskelkarte zum Zusammenstellen von Trainingsplänen. Klicke auf Muskeln in einer anatomischen SVG-Grafik und erhalte passende Übungen mit primären und sekundären Zielmuskeln.

Alles steckt in **einer einzigen HTML-Datei**. Kein Build-Schritt, keine Abhängigkeiten, kein Server. Einfach im Browser öffnen.

> 🇩🇪 Die MuscleMap ist komplett **auf Deutsch**: Muskel- und Übungsnamen sind deutsch, die Muskeln zusätzlich mit lateinischem Fachbegriff.

## Funktionen

- Anatomische SVG mit anklickbaren Muskelgruppen
- Übungsdatenbank (35 Übungen) mit primären und sekundären Zielmuskeln
- Deutsche und lateinische Muskelnamen
- Läuft komplett offline
- Schlank: eine kleine Datei, lädt sofort

## Benutzung

1. `form-muskelkarte(4).html` herunterladen
2. In einem beliebigen modernen Browser öffnen
3. Muskeln anklicken und passende Übungen ansehen

## Anpassen

Die Übungen liegen als einfaches JS-Array in der Datei:

```js
{
  "name": "Reverse Butterfly",
  "category": "Isolationsübungen",
  "group": "ruecken",
  "primary": ["deltoid_hinten"],
  "secondary": ["trapez_mitte_rhomboiden", "trapez_oben"]
}
```

- `primary` / `secondary` nutzen die Muskel-IDs aus der SVG (Attribut `data-muscle`)
- Für eine neue Übung einfach einen weiteren Eintrag ins Array setzen
- Jede verwendete Muskel-ID muss auch in der SVG existieren

## Technik

- Reines HTML, CSS und JavaScript
- Inline-SVG
- Keine Frameworks, keine externen Anfragen

## Lizenz

noch keine

## Autor

Lu Vobius
