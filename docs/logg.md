# Logg.md

## 24.02.25

### Planlegging

- se [her](https://github.com/Kireobat/testfagprove/blob/master/docs/plan.md)

### Backend - Oppsett

- Begynte på backend biten av applikasjonen, opprettet databasen, entiteter, dtoer, repo filer osv.

## 25.02.25

### Backend - Autentisering

- Satt opp login på backend med passord/mail og oauth fra github
- Satt opp rolle system
- Opprette, slette, endre, hente rom
- Begynte på samme funksjonaliteten for møter
- Klarte å committe secrets til git 🤡. Har nå endret secrets

## 26.02.25

### Backend - CRUD og Validering

- CRUD for møter med tidsvalidering og UpdateMeetingDto
- Ny ParticipantController + DTO-er for deltakerhåndtering
- Rettighetssjekk via hasSufficientRolePermissions() (boolean-basert)
- Datamodell: Direkte ID-referanser, nullable auth-felter, kaskadeslett
- Erstattet SQL med JPA Specifications for spørringer
- Fjernet ubrukt auth0-bibliotek
- Implementerte kaskadesletting av brukerdata med valg for sletting/overføring.
- Oppdaterte SQL-migrasjoner med sikkerhetssjekker.
- La til SYSTEM- og SLETTET-brukerkonti.
- Forenklet AuthService ved direkte rollehåndtering.
- Fikset tilgangskontroll ved å endre OR til AND i kontrollere.
- Forbedret entitetsrelasjoner og lagt til oppdateringsfunksjonalitet for brukere.
- Styrket feilhåndtering, kaskadeoperasjoner og tidsstempelhåndtering.
- Ryddet i kode og fjernet ubrukt kode.
- La til testdata-SQL-filer for databaseoppsett (OAuth-provider, roller, testbrukere).

## 27.02.25

### Backend - Fortsatt Utvikling

- Laget tester for alle service filer
- Endret møtebookings prosessen for å forhindre dobbeltbooking
- La inn jenkinsfile for CI/CD
- Gjordt api tilgjengelig for ved [https://api.kireobat.eu/fish-time](https://api.kireobat.eu/fish-time)

### Frontend - Oppsett

- Satt opp frontend prosjektet med Svelte 5, TailwindCSS og Flowbite UI med custom farger osv.
- Navbar for mobil og desktop
- Lagt inn kalender komponent
- Lagt inn backend via openapi-generator-cli
- Lagt inn legal jargin
