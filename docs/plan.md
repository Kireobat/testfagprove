# Plan.md

- [Plan.md](#planmd)
  - [powerpoint](#powerpoint)
  - [Hovedoppgave](#hovedoppgave)
    - [Logg](#logg)
    - [Fremdriftsplan](#fremdriftsplan)
    - [Planlegging](#planlegging)
      - [endepunkter jeg vil ha](#endepunkter-jeg-vil-ha)
      - [Databasestruktur](#databasestruktur)
      - [Teknologi valg](#teknologi-valg)
        - [Backend](#backend)
        - [Frontend](#frontend)
  - [Andre ting](#andre-ting)
    - [kompetansemål](#kompetansemål)
      - [1](#1)
      - [2](#2)
      - [3](#3)
      - [4](#4)
      - [5](#5)
      - [6](#6)
      - [7](#7)
      - [8](#8)
      - [9](#9)
      - [10](#10)
      - [11](#11)
      - [12](#12)
      - [13](#13)
      - [14](#14)
      - [15](#15)
      - [16](#16)
      - [17](#17)
      - [18](#18)
      - [19](#19)
      - [20](#20)
      - [21](#21)

## powerpoint

bruke [standard powerpoint](https://nettfisken.fiskeridirektoratet.no/ting-du-trenger/presentasjoner/standard-presentasjon-norsk-20250131.pptx) for fdir

## Hovedoppgave

### Logg

Logg er tilgjengelig [her](https://github.com/Kireobat/testfagprove/blob/master/docs/logg.md)

### Fremdriftsplan

| Dato(er) | Oppgave | Fremgangsmåte | Kompetansemål | Arbeidsverktøy | Kilder | Begrunnelse | Ref |
|-|-|-|-|-|-|-|-|
| **24.02.25** | Planlegge | Reflektere og tenke på hvordan jeg bør utføre oppgaven på en god måte. Dette inkluderer database stuktur, enkelte endepunkter, ideer til frontend. | [1](#1), [2](#2), [4](#4), [5](#5), [6](#6), [10](#10) | VSCode | Me, Myself & I | Det kan være lurt å ha en plan for hva man skal gjøre | [Lenke](#planlegging) |
|24.02.25|Planlegge databasestruktur|skrive + tenke|[5](#5)|dbdiagram.io||Det er greit ha en database når man skal lagre ting||
|24.02.25|Planlegge nødvendige endepunkter|skrive + tenke|[5](#5)|VSCode||Det er ofte praktisk å ha noen endepunkter slik at frontenden kan snakke med backenden||
|24.02.25|Søke etter ting jeg tror kan hjelpe med oppgaven|Bruke firefox og en søkemotor til å undersøke og finne forskjellige måter å gjøre gjennomføringen av oppgaven enklere|[6](#6), [10](#10)|Firefox|Github og andre nettsider|Jeg kan finne gode løsninger på problemer jeg vil møte||
|||||||||
| **25.02.25** |Begynne på backend| opprette prosjekt på git, sette opp spring applikasjon osv.||IntelliJ IDEA||||
| 25.02.25 |Sette opp git prosjekt| opprette prosjekt på git||IntelliJ IDEA, git||||
| 25.02.25 |Opprette spring applikasjon| opprette spring applikasjon||IntelliJ IDEA||||
| 25.02.25 |implementere databasestruktur| implementere databasestruktur||IntelliJ IDEA||||
| 25.02.25 |begynne på endepunkter| begynne på endepunkter||||||
| 25.02.25 |Lage Jenkinsfile og sjekke et jenkins fungerer| lag fil, push||IntelliJ IDEA||||
| 25.02.25 |Få alle endepunktene til å fungere| Få alle endepunktene til å fungere||IntelliJ IDEA||||
| 25.02.25 |Gjør backenden tilgjengelig på nett| Jenkins bygger og ber docker starte opp en container ||Jenkins, Docker||Det er nyttig at at apiet ditt er tilgjengelig å bruke||
|||||||||
| **26.02.25** |Fortsette på backend| lage og sjekke at endepunkter fungerer ||IntelliJ IDEA||||
|||||||||
| **27.02.25** |Begynne på frontend| lage en frontend i svelte? bruk openapi-generator-cli for api||VSCode||||
| 27.02.25 |Sette opp git prosjekt| opprette prosjekt på git||VSCode, git||||
| 27.02.25 |Sette opp prosjekt med nødvendige avhengigheter| opprette prosjekt med nødvendige avhengigheter||VSCode||||
| 27.02.25 |Generer api| `npm run openapi:all`||VSCode, npm||||
|||||||||
| **28.02.25** |Fortsette på frontend|||||||
|||||||||
| **01.03.25** |Fikse alle feilene| Jeg kommer til å fokusere på det jeg ser er nødvendig/viktigst 28.02.25|[15](#15), [16](#16)|||||
|||||||||
| **02.03.25** |Fikse alle feilene||[15](#15), [16](#16)|||||
|||||||||
| **03.03.25** |Fikse alle feilene, men nå med dårligere tid||[15](#15), [16](#16)|||||

### Planlegging

Applikasjons navn: **FishTime**

Logo

#### endepunkter jeg vil ha

- /meetings/create
  - title
  - description
  - time
  - room
  - participants
- /meetings/update
- /meetings/delete
  - ?id
- /meetings
  - ?id
  - ?startTime
  - ?endTime
  - ?search
  - ?createdBy
  - ?participants
- /rooms/create
- /rooms/delete
- /rooms/update
  - mulighet til å aktivere/deaktivere
  - endre navn, plassering osv.
- /users
  - ?name
  - ?id
- /login
  - oauth eller brukernavn/passord
- /logout

#### Databasestruktur

[Lenke](https://dbdiagram.io/d/fish_time-67bc3003263d6cf9a03767a9)

#### Teknologi valg

##### Backend

- Kotlin
  - Er som java, men mindre verbost
- Springboot
  - Det jeg har erfaring med fra fdir
- Swagger UI
  - Enkel måte å få oversikt og dokumentere endepunktene sine på
- Postgres
  - Har brukt det i andre sammenhenger i fdir

##### Frontend

- Svelte 5?
  - Mindre verbos, ligner mer på ren html, compilet på server side
- Tailwind CSS
  - Er det jeg bruker for CSS på frontend
- Flowbite UI
  - UI lib som er kompatibelt med Svelte 5
- Openapi Generator Cli
  - Tar seg av api og dto oppretting på frontend, reduserer hvor mye kode man må skrive
- [https://github.com/vkurko/calendar](https://github.com/vkurko/calendar)

## Andre ting

### [kompetansemål](https://www.udir.no/lk20/iuv03-01/kompetansemaal-og-vurdering/kv530)

#### 1

planlegge, utvikle og dokumentere løsninger med innebygd personvern og sikkerhet

#### 2

planlegge, utvikle og dokumentere løsninger som er energieffektive og bærekraftige

#### 3

videreutvikle en løsning for å ivareta brukernes behov

#### 4

planlegge, utvikle, sette opp og dokumentere systemer for datainnsamling, analyse og visualisering

#### 5

planlegge, utvikle, sette opp og dokumentere integrasjoner mellom ulike systemer og databaser

#### 6

utvikle og bruke dokumentasjon og veiledninger

#### 7

veilede brukere i ulike oppgaver

#### 8

håndtere påloggingsopplysninger på en sikker og forsvarlig måte

#### 9

utvikle og tilpasse brukergrensesnitt som ivaretar krav til universell utforming

#### 10

velge og bruke relevante rammeverk og moduler til utvikling

#### 11

beskrive konsekvenser av teknisk gjeld i løsninger

#### 12

beskrive hvilke krav som ulike løsninger stiller til infrastruktur, og hvilke muligheter og begrensninger som følger av infrastrukturen

#### 13

gjøre rede for og anvende gjeldende regelverk for personvern, opphavsrett og informasjonssikkerhet i eget arbeid

#### 14

bruke utviklingsstrategier og samarbeide med andre utviklere

#### 15

feilsøke kode og rette feil i algoritmer og kode

#### 16

utforske prosesser knyttet til testing og feilsøking i utvikling av løsninger

#### 17

behandle bedriftsinterne opplysninger på en sikker og etisk forsvarlig måte

#### 18

utforske konseptene maskinlæring og kunstig intelligens

#### 19

utforske og vurdere eksisterende og nye teknologier og bransjerelevante kodespråk

#### 20

reflektere over og beskrive hvordan teknologi kan misbrukes og påvirke samfunnet negativt

#### 21

gjøre rede for hvilke krav og forventninger som stilles til et likeverdig og inkluderende yrkesfellesskap, og reflektere over hvilke plikter og rettigheter arbeidsgiver og arbeidstaker har i lærebedriften
