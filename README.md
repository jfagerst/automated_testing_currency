# Automaattinen testaus – Currency, osat 1–4

Tämä repositorio sisältää Ohjelmistotestaus-kurssin tehtävän Automated testing – Currency, osat 1–4.

Projektissa on yksinkertainen valuuttamuunninsovellus, joka hakee valuuttakursseja julkisesti saatavilla olevan rajapinnan kautta. Tehtävien tavoitteena on harjoitella automaattista testausta sovelluskehityksessä.

Projektin testaus kattaa seuraavat osa-alueet:

- Osa 1: Vite- ja Vitest-ympäristön käyttöönotto sekä yksinkertainen yksikkötesti.
- Osa 2: Yksikkötestaus mockien, stubien ja spy-toimintojen avulla.
- Osa 3: API-kutsujen simulointi testeissä.
- Osa 4: API-testaus.



## Käyttöönotto

Backend-palvelin toimii osoitteessa http://localhost:3000 ja frontend osoitteessa http://localhost:5173.

Asenna riippuvuudet sekä projektin juuressa että `server`-kansiossa suorittamalla kummassakin: 
`npm i` 

Jos backendin riippuvuuksia puuttuu, ne voi asentaa `server`-kansiossa komennolla:
`npm i express cors dotenv`

## Sovelluksen käynnistäminen

Siirry `server`-kansioon ja käynnistä backend kehitystilassa: 
`npm run dev` tai `npm run start`. 

Siirry projektin juurikansioon ja käynnistä frontend: 
`npm run dev`.

## API testaaminen REST Clientillä

1. Käynnistä backend server-kansiossa komennollla `npm run dev` tai `npm run start`. 
2. Avaa tiedosto `server/test.rest` editorissa, jossa REST Client -laajennus on käytettävissä.
3. Suorita pyyntö painamalla testikoodin yläpuolella näkyvää Send Request -toimintoa.

## Backendin testien suorittaminen Vitestillä

Siirry `server`-kansioon ja suorita testit komennolla:

`npm run test`

## Testikattavuusraportin luominen

Testikattavuusraportin voi luoda server-kansiossa komennolla:

`npm run coverage`

Jos coverage-riippuvuudet on asennettu ja testiajo tuottaa raportin, raportti löytyy server/coverage-kansiosta. Avaa kansion index.html selaimessa tarkastellaksesi raporttia.





