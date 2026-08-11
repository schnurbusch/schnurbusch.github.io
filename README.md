# Schnurbusch Games, Website

Statische Portfolio- und Produktseite. Zweck: eine Publisher-Website, die Unitys
Content-Transparency-Regel **Abschnitt 1.7.2** erfüllt, nachdem ChipForge am
11.08.2026 abgelehnt wurde, weil `schnurbusch.itch.io` als Website hinterlegt war.

## Warum der Aufbau so ist

Unity verbietet Marktplatz-Profile als Publisher-Website und verbietet Kauffunktionen
auf der **Startseite**. Erlaubt sind eigene Seiten, bei denen die Kaufseiten eine Ebene
tiefer liegen. Deshalb gilt hier:

- `index.html` enthält **keine** Store-Links, **keine** Preise, **keine** Kauf-Buttons.
  Nur Produktname, eine Zeile Beschreibung und einen Link auf die Detailseite.
- Die Store-Links stehen ausschließlich in den Detailseiten, im Block
  „Where to get it" ganz unten.

**Diese Trennung nicht aufweichen.** Kein „Jetzt kaufen" auf die Startseite, keine
Preise in die Kacheln.

## Dateien

| Datei | Inhalt |
|---|---|
| `index.html` | Startseite: Tools, Games, About |
| `chipforge.html` `loclayer.html` `portraitfit.html` `hintonce.html` | Produktseiten |
| `famechaser.html` | Spiel, plus woher die Tools stammen |
| `style.css` | gemeinsames Stylesheet |
| `img/` | Cover-Bilder, aus den `*_Publishing`-Ordnern kopiert |

Farben identisch zur itch-Storefront: BG `#0f171b`, Panel `#16242c`, Text `#e6edf0`,
Akzent `#59d9f2`. Kein Build-Schritt, keine Abhängigkeiten, kein JavaScript.

## Lokal ansehen

`index.html` doppelklicken. Mehr braucht es nicht.

## Veröffentlichen über GitHub Pages

Kostenlos, dauerhaft, ohne Kreditkarte. Ohne Git-Kenntnisse, rein über die Weboberfläche:

1. Account auf <https://github.com> anlegen. Der Benutzername wird Teil der Adresse,
   also einen wählen, den man auch in Bewerbungen zeigen mag.
2. **New repository** anlegen, Name exakt `BENUTZERNAME.github.io`, Sichtbarkeit
   **Public**, kein README ankreuzen.
3. Im leeren Repository auf **uploading an existing file** klicken, dann den kompletten
   Inhalt dieses Ordners hineinziehen, den Unterordner `img` inklusive. `README.md`
   kann mit hoch, sie stört nicht.
4. **Commit changes**.
5. Nach ein bis zwei Minuten ist die Seite unter `https://BENUTZERNAME.github.io`
   erreichbar.

## Danach im Unity Publisher Portal

Profil öffnen, im Feld für die Website die itch-Adresse durch die neue Adresse
ersetzen, speichern. Erst dann die abgelehnten und wartenden Pakete erneut einreichen.

## Pflege

Sobald ein Paket im Asset Store freigegeben ist, in der jeweiligen Produktseite im
Block „Where to get it" den Status `in review` durch einen Link auf die Asset-Store-Seite
ersetzen.
