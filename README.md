# Woordkaarten

Een eenvoudige flashcard-app om talen te leren. Klik op een kaart en ze draait om naar de vertaling. Werkt in de browser en kan als app geïnstalleerd worden op pc en gsm (PWA), ook offline.

## Functies

- Omdraaibare kaarten (klik of spatie)
- Meerdere stapels, elk met een eigen taalpaar
- Kaarten toevoegen, verwijderen en importeren (`voorkant;achterkant`, één per regel)
- Herhaling volgens het Leitner-systeem (na 1, 2, 4, 8 en 16 dagen)
- Uitspraak via de Web Speech API
- Omgekeerd oefenen
- Licht en donker thema
- Werkt offline en is installeerbaar

## Gebruiken

Open de gehoste pagina of start een lokale server in deze map:

```bash
python3 -m http.server 8000
```

Ga daarna naar `http://localhost:8000`.

## Online zetten

**GitHub Pages:** upload de bestanden naar een repository, ga naar *Settings → Pages* en kies de `main`-branch.

**Netlify:** sleep de map op [app.netlify.com/drop](https://app.netlify.com/drop).

Een PWA heeft HTTPS nodig. Beide diensten leveren dat gratis.

## Installeren

- **Android (Chrome):** menu → *App installeren*
- **iPhone (Safari):** Delen → *Zet op beginscherm*
- **Pc (Chrome/Edge):** installeer-icoontje in de adresbalk

## Bestanden

| Bestand | Doel |
| --- | --- |
| `index.html` | De volledige app (HTML, CSS en JavaScript) |
| `manifest.json` | Naam, kleuren en iconen voor installatie |
| `sw.js` | Service worker voor offline gebruik |
| `icon-192.png`, `icon-512.png` | App-iconen |

## Gegevens

Alle kaarten staan lokaal in `localStorage` van je browser. Wis je de browserdata, dan verdwijnen ze. Gebruik *Kopieer als tekst* in een stapel voor een reservekopie. Verhoog `CACHE` in `sw.js` als je de bestandslijst wijzigt.

## Plannen

- Synchronisatie via Google Drive (`drive.appdata`)

## Licentie

[MIT](LICENSE)
