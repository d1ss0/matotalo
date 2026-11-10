# Matotalo – yhteinen

Selainpeli, jossa rakennetaan matojen talo maan alle. Perustuu lapsen piirrokseen.

- Yksi tiedosto: `index.html` (ei taustapalvelinta, ei käännösvaihetta)
- Peli tallentuu selaimen localStorageen laite- ja osoitekohtaisesti
- Fontti (Patrick Hand) ladataan Google Fontsista; ilman verkkoa käytetään varafonttia

## Ajaminen

Avaa `index.html` selaimessa tai tarjoile se millä tahansa staattisella web-palvelimella:

```
python3 -m http.server 8080
```

## Docker

```
git pull
docker compose up -d --build
```

Portit ja verkot kuuluvat omaan tiedostoosi `docker-compose.override.yml`, jota ei viedä repoon.
Docker Compose yhdistää sen automaattisesti. Esimerkiksi portin julkaisu:

```
services:
  matotalo:
    ports:
      - "8080:80"
```

Tabletilla: avaa osoite selaimessa ja valitse "Lisää Koti-valikkoon", niin peli
aukeaa omasta kuvakkeestaan koko näytöllä.

## Sisältö tällä hetkellä

- 21 ruudun levyinen metsä, josta putoaa lehtiä, vapaa kamera (veto, nipistys, 🔍, 🏠)
- Vuorokausi ja valaistus, neljä vuodenaikaa (2 pelipäivää / vuodenaika)
- Tapahtumat: sade, kuivuus, rastas, myyrä
- Huoneet: keittiö, ruokakomero, makuuhuone, kylpyhuone, kellari, lastenhuone, lääkäri, olohuone, askarteluhuone, takkahuone, salainen huone
- Talvi: pakkasraja, ilmainen kaivuu, aarteet, lumikasat
- Isot huoneet avautuvat matomäärän mukaan: uloskäytävä (10), suurkeittiö ja makuusali (15), suurvarasto (20)
- Ääniefektit WebAudiolla (ei äänitiedostoja), mykistys 🔊-napista

## Seuraavaksi

- Yhdyskunnan kasvu ja virstanpylväät
- Talvijuhla
- Lisää petoja ja viimeistelyä
