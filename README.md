# Episode Visit Notes — GitHub Pages

## Bestanden
`index.html` (de hele app) · `manifest.webmanifest` · `sw.js` (offline) · `icon-*.png` · `.nojekyll`

Alles moet in de **hoofdmap** van de repo staan, niet in een submap.

## Online zetten
1. github.com → **New repository**. Naam: `visits`. Zet op **Public** (bij een private repo werkt Pages niet op het gratis plan). Create.
2. Op de lege repo-pagina: **uploading an existing file**. Sleep de **inhoud** van deze map erin (de losse bestanden, niet de map zelf). **Commit changes**.
3. **Settings → Pages**. Bij *Source*: **Deploy from a branch**. Branch: `main`, map `/ (root)`. **Save**.
4. Wacht 1-2 minuten. Bovenaan die pagina komt je URL: `https://<jouw-account>.github.io/visits/`.

Ziet stap 2 het bestand `.nojekyll` niet (sommige browsers laten dotfiles vallen)? Dan: **Add file → Create new file**, naam `.nojekyll`, leeg laten, commit. Klaar.

## Installeren op de telefoon
Open de URL in **Chrome** (Android) → ⋮ → **App installeren** of **Toevoegen aan startscherm**. Daarna open je hem via het icoon: volledig scherm, werkt offline.

iPhone/Safari: deelknop → **Zet op beginscherm**.

## Updaten
Nieuwe versie van mij = in de repo op `index.html` klikken → potloodje → oude inhoud vervangen. Of **Add file → Upload files** en `index.html` overschrijven. Binnen een minuut live; je notities blijven staan.

Bij een grotere update lever ik ook een nieuwe `sw.js` — die dan meeuploaden, anders houdt de telefoon de oude versie in de cache.

## Belangrijk over je data
- Notities staan **op het toestel**, in de browseropslag onder deze URL. Niet op GitHub.
- Zolang de URL gelijk blijft, blijft de data staan — ook na afsluiten, herstarten, offline.
- Weg bij: site-gegevens wissen, app verwijderen, ander toestel, incognito.
- Kom je van Netlify? De data verhuist **niet** mee. Eerst daar exporteren (Instellingen → Export), dan hier importeren.
- Exporteer wekelijks een JSON naar OneDrive of SharePoint als backup.
- Iedere collega installeert dezelfde URL en heeft zijn eigen lokale notities. Geen automatische sync.

## Eigen domein (optioneel)
Wil je `visits.episode.eu`: Settings → Pages → *Custom domain*. IT zet één CNAME-record. Let op: dat verandert de URL, dus doe het vóór je echt notities gaat maken, of exporteer eerst.
