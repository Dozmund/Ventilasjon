# Ventilasjon - Work In Progress

Statisk utkast til et lesegrensesnitt for ventilasjonswikien. Ingen byggesteg eller backend kreves.

## Åpne utkastet

Start en lokal webserver i mappen: `python -m http.server 8765`.
Åpne http://localhost:8765.

## Innhold

- Responsiv forside, sidemeny og søk i ni fagområder og artikkelteksten deres.
- Tolv innebygde wikiartikler, inkludert maler og vedlikehold.
- Artikkelvisning med tabeller, kodeblokker og lenke til redigering i GitHub Wiki.
- Søk og artikkelvisning fungerer uten eksterne API-kall.
- Google Fonts brukes til skrifter, med lokale reserveskrifter.
- Ingen analyseverktøy, kontoer eller skjemaer.

Dette er et designutkast. Produktregister og enkelte fagveiledninger er fortsatt utkast slik de er i wikien.

## Publiser med GitHub Pages

Utkastet ligger på grenen `utkast/github-pages`.

1. Se gjennom og eventuelt flett grenen til `main`.
2. Åpne repository Settings > Pages.
3. Velg Deploy from a branch, aktuell gren og / (root).
4. Lagre. Forventet adresse er https://dozmund.github.io/Ventilasjon/.

Pages er ikke aktivert som del av dette utkastet.

## Oppdatere innholdet

Siden viser en kopi av wikien fra 18.11.2026. Endringer i GitHub Wiki vises ikke automatisk.

Klon eller oppdater wikien separat og kjør:

```text
git clone https://github.com/Dozmund/Ventilasjon.wiki.git
node sync-wiki.cjs <sti-til-wiki-klone>
```

Commit og push oppdatert `content.js` til Pages-grenen.

Nye artikler inkluderes i innholdsfilen. Legg dem også til i emneoversikten eller ekstralenkene i `app.js` for å gjøre dem synlige i navigasjonen. Den enkle Markdown-visningen støtter formatene som brukes i startartiklene, ikke hele Markdown-spesifikasjonen.

## Videre valg

- Godkjenne visuell retning og navn.
- Legge til offisiell logo ved behov.
- Avgjøre om automatisk synkronisering fra wiki skal settes opp.
