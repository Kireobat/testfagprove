# vurdering.md

## Backend

Backend applikasjonene jeg har utviklet er laget i Kotlin med Spring Boot. Jeg har brukt Swagger UI for å dokumentere endepunktene mine. Dette har gjort det enklere å få oversikt over endepunktene og hvordan de henger sammen. Jeg har brukt Postgres som database, da jeg har erfaring med det fra tidligere prosjekter.

Jeg har alle endepunktene jeg trenger for å administrere booking av møter, innlogging, registrering, oauth, brukere og rom. All grunleggende funksjonalitet er på plass slik den er beskrevet i planen.

Hvis man vil videreutvikle denne applikasjonen kan man begynne med å legge til varsler. For dette må man nok integrete mot tjenester som Sendgrid eller lignende. De andre forbedringene man kan gjøre er stort sett relatert til frontend.

## Frontend

Frontend applikasjonen er laget i Svelte 5 med TailwindCSS og Flowbite UI. Jeg har laget en navbar som fungerer både på mobil og desktop. Jeg har lagt inn en kalender komponent som gjør det enkelt å se hvilke møter som er satt opp. Jeg har også lagt inn backend via openapi-generator-cli, slik at frontend kan snakke med backend.

Kalender visningen av møter kan i framtiden forbedres med filter slik at man f.eks bare ser møter man selv er med i. Denne funksjonaliteten er allerede implementert i backend, men ikke i frontend. I tillegg er det mye av designet og fargevalget som kan forbedres. Frontenden er heller ikke særlig mobil vennelig, så det er også et forbedringspunkt.
