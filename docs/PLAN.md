# Projektplan: Min Helseassistent

## 1. Kravoppsummering
- Helseapp for å holde oversikt over egen helse.
- Brukeren skal kunne loggføre symptomer, måleverdier, søvn og humør.
- Brukeren skal få oversikt over sine data gjennom grafer og rapporter.
- Innebygde påminnelser og varslinger.
- Tillegg (valgfritt): brukerinnlogging, deling, integrasjon mot eksterne API-er.

## 2. Hovedleveranser (fire større oppgaver)
1. **Grunnleggende prosjektoppsett**  
   Oppsett av repository, utviklingsmiljø, CI, arkitektur og designskisser.
2. **Helse- og symptomlogg**  
   Skjema for registrering av symptomer, måleverdier, søvn og humør, med lokal lagring og validering.
3. **Varsler og målsettinger**  
   Modul for påminnelser, mål- og habit-tracking, samt konfigurering av push-varsler.
4. **Dataanalyse og deling**  
   Visualisering av data, rapporteksport, og frivillig funksjonalitet for deling/integrasjoner.

## 3. Kanban for Oppgave 2: "Helse- og symptomlogg"

| Kolonne | Kort | Beskrivelse | Test/Verifikasjon |
| --- | --- | --- | --- |
| **Backlog** | UX-LOGG-01 | Skisser registreringsflyt og skjemaer. | Wireframes signert av produktansvarlig. |
| **Backlog** | DATA-LOGG-02 | Definer datamodell for helseoppføringer. | Enhetstester dekker feltvalidering. |
| **Klar til å starte** | API-LOGG-03 | Avklar lagring (lokalt/sky) og API-kontrakter. | Godkjent teknisk design-notat. |
| **I arbeid** | UI-LOGG-04 | Implementer skjerm for symptomregistrering med validering. | Manuell test: registrere og se oppsummering. |
| **Under test** | TEST-LOGG-05 | Lag automatiserte tester (enhet + integrasjon). | Kommando `npm test logbook` passerer. |
| **Utført** | DOC-LOGG-06 | Oppdater dokumentasjon og release-notat. | Pull request godkjent og merget. |

## 4. Milepæler og avhengigheter
- Oppgave 1 må ferdigstilles før Oppgave 2 kan starte (miljø og design må være klart).
- Oppgave 2 og 3 kan kjøres parallelt etter at grunnoppsettet er klart.
- Oppgave 4 avhenger av dataene fra Oppgave 2 for visualisering.

## 5. Teststrategi
- **Kontinuerlig integrasjon:** Kjør enhetstester på hver commit.
- **Designgjennomganger:** Valider tidlig med interessenter.
- **Brukertesting:** Korte brukerøkter for å verifisere registreringsflyten og varslingsfunksjonen.
- **Måledata:** Test med både manuelle og automatiserte datasett for å sikre korrekte grafer.

