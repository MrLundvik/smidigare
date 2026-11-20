# Smidigare

Ett rörlighetsprogram för hemmabruk, byggt för en otränad och stel kropp, med lite extra fokus på golf. Appen ger ett dagligt pass på max 45 minuter, loggar det du gör och anpassar övningarna efter hur det går.

Allt ligger i en enda HTML-fil. Det finns ingen server, inget konto och inget byggsteg.

**Adress:** <https://mrlundvik.github.io/smidigare/>

## Installera på telefonen

1. Öppna adressen ovan i **Chrome** på telefonen.
2. Välj menyn **⋮ → Installera app** (eller *Lägg till på startskärmen*).

Appen startar sedan som en vanlig app och fungerar även utan internet.

Repot är publikt eftersom GitHub Pages är gratis för publika repon. Ingen träningsdata hamnar i repot.

## Var sparas mina data?

All data sparas **lokalt i webbläsaren på telefonen** (localStorage), aldrig på GitHub.

- **Säkerhetskopia till Google Drive:** gå till **Inställningar → Säkerhetskopia till Google Drive → Spara till Google Drive**. Välj *Drive* i Androids delningsmeny och sedan mapp. Appen påminner dig om det har gått mer än 7 dagar sedan senaste kopian.
- **Återställ** (ny telefon eller rensad webbläsare): gå till **Återställ från fil** och välj filen i Drive i filväljaren. Poster som redan finns läggs inte till två gånger.
- Som reserv går det också att kopiera säkerhetskopian som text.
- Versionen på claude.ai sparar sina data separat, på ditt Claude-konto. Data kan flyttas mellan versionerna med samma säkerhetskopia.

## Programmet

| Dag | Pass |
|---|---|
| Mån | Ben och höft: styrka i fullt rörelseomfång + höftrörlighet |
| Tis | Rörlighet |
| Ons | Överkropp och bål + ned och upp från golvet |
| Tor | Rörlighet |
| Fre | Golf och rotation |
| Lör | Lätt pass + promenad |
| Sön | Vila |

Det finns också ett eget pass, **Före golfrundan**, med cirka 10 min dynamisk uppvärmning före spel.

- **Faser:** Fas 1 (v. 1–4) 2 × 30 s stretch och 2 × 8–10 styrka. Fas 2 (v. 5–8) 2 × 45 s och 2 × 10–12. Fas 3 (v. 9–16) 2 × 60 s och 3 × 10–12. Du går upp en fas efter 4 veckor om du har tränat minst cirka 3 dagar i veckan.
- **Övningssteg:** varje övning har 3 steg. Tre gånger *Lätt* i rad flyttar den upp ett steg. *Tungt* två gånger, eller *Gjorde ont*, flyttar den ned ett steg. Steg som kräver golvet är spärrade tills du slår på det i inställningarna.
- **Tester var 4:e vecka:** sitt och räck, rygg-klia och 30 s uppresning (Senior Fitness Test), sittande rotation, enbensstående, valfritt sitting-rising test, vikt och midjemått.
- **Promenader** ligger utanför 45-minuterstaket. Veckomålen är 2 intervallpromenader och 1 promenad i backe eller trappor, och det finns en inbyggd intervallguide.
- **Dags att uppdatera:** när de flesta övningar är på högsta steget, eller efter 8 veckor i fas 3, säger appen till. Den ger då en sammanfattning som du kan klistra in hos Claude för att få nästa nivå.

## Uppdatera appen

Appen publiceras med GitHub Pages från grenen `main`, mappen `/` (root). Ändringar som pushas till `main` ligger ute efter en till två minuter.

1. Ersätt `index.html` i repot med den nya versionen.
2. Öka versionen i `sw.js` (`const CACHE = "smidigare-v4"` → `v5`).

Telefonen hämtar den nya versionen nästa gång appen öppnas med internet. Ibland behöver appen stängas och öppnas en gång till.

## Kunskapsunderlag

- ACSM:s riktlinjer för rörlighetsträning (2–3 dagar/vecka som minimum, dagligen mest effektivt; 30–60 s håll)
- WHO:s riktlinjer för fysisk aktivitet 2020 (150–300 min måttlig aktivitet, styrka minst 2 dagar, balans för äldre)
- Thomas m.fl. 2018: dos–respons för stretching (minst 5 min per muskelgrupp och vecka)
- Feland m.fl. 2001: 60 s håll ger större effekt hos äldre
- Afonso m.fl. 2021: styrketräning ger rörlighetsvinster jämförbara med stretching
- Rikli & Jones: Senior Fitness Test; Araújo: sitting-rising test

## Viktigt

Appen ersätter inte vård. Rådfråga läkare eller fysioterapeut innan du börjar om du har hjärt- eller kärlsjukdom, högt blodtryck, diabetes eller nyligen har opererats. Avbryt vid bröstsmärta, yrsel, ovanlig andnöd eller skarp, strålande smärta.
