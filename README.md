# TERRA

Indovina il paese del giorno in 8 tentativi. Ogni paese provato viene confrontato con quello nascosto su nove caratteristiche: continente, popolazione, superficie, PIL pro capite, età media, aspettativa di vita, paesi confinanti, sbocco sul mare, senso di guida. Verde se coincide, rosso se no, freccia su o giù per i valori numerici. Un riquadro in alto riassume quanto scoperto (valori trovati, intervalli, esclusioni). Paese del giorno uguale per tutti, più allenamento. Interfaccia in italiano e inglese.

Pubblicato su https://dailygames-hub.github.io/terra/ come parte di Daily Games.

## Dati

`data.js` contiene i 193 stati membri ONU. Fonti:

- popolazione, età media, aspettativa di vita, PIL pro capite (a parità di potere d'acquisto): [CIA World Factbook](https://www.cia.gov/the-world-factbook/) via [factbook/factbook.json](https://github.com/factbook/factbook.json), pubblico dominio, stime 2024/2025;
- superficie, paesi confinanti, sbocco sul mare, continente (classificazione ONU), nomi e traduzioni: [mledoze/countries](https://github.com/mledoze/countries), licenza ODbL;
- senso di guida: [samayo/country-json](https://github.com/samayo/country-json), licenza MIT.

Continenti: Africa, Asia, Europa, Nord America (comprende America Centrale e Caraibi), Sud America, Oceania. Per aggiornare i dati basta rigenerare `data.js` con lo stesso formato (vedi l'intestazione del file).

## Cose da personalizzare

Nel blocco `CONFIG` in cima allo script di `index.html`: `NAME`, `SITE_URL` (aggiunto al testo condiviso), `EPOCH` (la data del giorno 1: cambiarla cambia la sequenza dei paesi) e `TRIES`.

## Fonti e licenze

- Codice: licenza MIT (vedi `LICENSE`). I dati seguono le licenze delle rispettive fonti indicate sopra.
- Carattere: [Familjen Grotesk](https://github.com/Familjen-Sthlm/Familjen-Grotesk), SIL Open Font License 1.1 (`fonts/OFL.txt`), sottoinsieme latino.
- Meccanica della famiglia dei giochi "indovina confrontando gli attributi"; nome, grafica, codice e dataset sono originali.

## File

```
index.html    il gioco
data.js       i 193 paesi con le nove caratteristiche
game.json     scheda per la landing page di Daily Games
preview.svg   anteprima per la landing page
favicon.svg   icona
fonts/        carattere Familjen Grotesk e licenza
```
