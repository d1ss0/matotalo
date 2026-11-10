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

## Sisältö tällä hetkellä

- 21 ruudun levyinen puutarha, vapaa kamera (veto, nipistys, 🔍, 🏠)
- Vuorokausi ja valaistus, neljä vuodenaikaa (2 pelipäivää / vuodenaika)
- Tapahtumat: sade, kuivuus, rastas, myyrä
- Huoneet: keittiö, ruokakomero, makuuhuone, kylpyhuone, kellari, lastenhuone, lääkäri, olohuone, askarteluhuone, takkahuone, salainen huone
- Talvi: pakkasraja, ilmainen kaivuu, aarteet, lumikasat

## Seuraavaksi

- Yhdyskunnan kasvu ja virstanpylväät
- Talvijuhla
- Lisää petoja ja viimeistelyä (äänet, hiukkaset)
