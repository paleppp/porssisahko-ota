# Pörssisähkö-näyttö – ohjelmistopäivitykset

Tämä repositorio jakaa **Pörssisähkö-näytön** (ESP32-2424S012C) valmiit ohjelmistoversiot.
Laitteet tarkistavat uusimman version automaattisesti öisin klo 3–5 osoitteesta

    https://github.com/paleppp/porssisahko-ota/releases/latest/download/manifest.json

ja asentavat sen, jos se on uudempi kuin laitteessa oleva versio.

## Turvallisuus

- Jokainen julkaisu on **allekirjoitettu** (ECDSA P-256). Laite asentaa vain tiedoston,
  jonka allekirjoitus täsmää laitteeseen käännettyyn julkiseen avaimeen ja jonka
  SHA-256-tarkiste vastaa manifestia.
- Jos uusi versio ei käynnisty kunnolla, laite palaa automaattisesti edelliseen versioon.
- Automaattiset päivitykset voi kytkeä pois laitteen asetussivulta (*Laite → Automaattiset päivitykset*).

## Manuaalinen asennus

Lataa julkaisun `.bin`-tiedosto ja asenna se laitteen asetussivulta:
*Laite → Päivitä tiedostosta*.
