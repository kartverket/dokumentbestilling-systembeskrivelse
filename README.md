# Tinglyste dokumenter API

APIet gir tilgang til en tjeneste som lar deg bestille og motta tinglyste dokumenter digitalt. For å bruke APIet, må organisasjonen din være registrert hos Digdir og ha blitt lagt til i APIet via Kartverket.

## Komme i gang

For å bruke APIet, må du først registrere organisasjonen din hos Digdir og hente et maskinporten-token som kreves for å autentisere API-kallene dine.

### Registrering hos Digdir

For å registrere organisasjonen din hos Digdir, opprett en brukerkonto og følg instruksjonene på [Digdir sin nettside](https://digdir.no/). Dette krever at du har en gyldig norsk virksomhet med et organisasjonsnummer.

### Autentisering med maskinporten-token

APIet bruker [Maskinporten](https://docs.digdir.no/docs/Maskinporten/maskinporten_overordnet) for autentisering. Følg Digdir sine instrukser for å få utstedt et token. Instruksjoner finner du på [dokumentasjon for API-konsument](https://docs.digdir.no/docs/Maskinporten/maskinporten_guide_apikonsument) hos Digdir.

## Funksjonalitet

APIet lar deg bestille tinglyste dokumenter ved å sende en forespørsel til APIet. Forespørselen må inneholde informasjon om hvilket dokument du ønsker å motta. Når du mottar en gyldig respons fra APIet, inneholder den en lenke til dokumentet som du kan laste ned.

## Bruk av Swagger

Swagger-dokumentasjonen for APIet gir deg en detaljert oversikt over alle API-kallene og tilhørende parameter-informasjon. Åpne [Swagger-dokumentasjonen (Kommer snart)](https://dokumentbestilling.kartverket.no/swagger-ui.html) i en nettleser for å bruke Swagger. Velg deretter ønsket API-kall, legg inn nødvendige parametere og send forespørselen. APIet behandler forespørselen og returnerer responsen tilbake til deg.

## Begrensninger

APIet har følgende begrensninger:

*   Kun tilgjengelig for kunder som er registrert hos Digdir og har organisasjonen sin lagt til i APIet.
*   Krever et gyldig maskinporten-token som har begrenset varighet og må fornyes regelmessig for å opprettholde tilgangen til APIet.
*   Gir kun tilgang til en håndfull tinglyste dokumenter som er tilgjengelige digitalt. For å få tilgang til andre dokumenter må du bestille disse på [Kartverket sine nettsider](https://www.kartverket.no/eiendom/bestille-fra-grunnboken).

## Feilhåndtering

APIet vil returnere ulike feilkoder og feilmeldinger avhengig av typen feil som oppstår. Disse er beskrevet i [Swagger-dokumentasjonen (Kommer snart)](https://dokumentbestilling.kartverket.no/swagger-ui.html).
