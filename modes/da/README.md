# career-ops -- Danske modes (`modes/da/`)

Denne mappe indeholder danske oversættelser af de vigtigste career-ops-modes for kandidater, der søger roller i Danmark eller arbejder med danske jobopslag.

## Hvornår skal disse modes bruges?

Brug `modes/da/`, hvis mindst én af disse betingelser er opfyldt:

- Du søger primært **danske jobopslag** (Jobindex, The Hub, danske karrieresider, LinkedIn DK)
- Dit **CV er på dansk**, eller du skifter mellem dansk og engelsk afhængigt af opslaget
- Du vil have svar og ansøgningstekster i **naturligt tech-dansk**, ikke maskinoversat tekst
- Du skal forholde dig til **danske kontraktvilkår** som overenskomst, pension, feriepenge, prøvetid, opsigelsesvarsel eller fastansættelse

Hvis de fleste opslag er på engelsk, så brug standard-modes i `modes/`. De fungerer fint i Danmark, men de kender ikke de danske markedsdetaljer lige så godt.

## Sådan aktiverer du dem

### Mulighed 1 -- pr. session

Sig i starten af sessionen:

> "Brug de danske modes under `modes/da/`."

eller

> "Vurder og skriv ansøgninger på dansk -- brug `modes/da/_shared.md` og `modes/da/tilbud.md`."

### Mulighed 2 -- permanent via profil

Sæt dette i `config/profile.yml`:

```yaml
language:
  primary: da
  modes_dir: modes/da
```

Mind agenten om at respektere feltet første gang ("Se i `profile.yml`, jeg har sat `language.modes_dir`").

## Hvilke modes er oversat?

Denne første iteration dækker de fire vigtigste modes:

| Fil | Oversat fra | Formål |
|-----|-------------|--------|
| `_shared.md` | `modes/_shared.md` | Delt kontekst, arketyper, globale regler, danske markedsforhold |
| `tilbud.md` | `modes/oferta.md` | Fuld vurdering af ét jobopslag (blok A-F) |
| `ansoeg.md` | `modes/apply.md` | Live-assistent til ansøgningsformularer |
| `pipeline.md` | `modes/pipeline.md` | URL-indbakke / second brain til gemte opslag |

De øvrige modes (`scan`, `batch`, `pdf`, `tracker`, `auto-pipeline`, `deep`, `contacto`, `ofertas`, `project`, `training`) bliver ved med at bruge EN/ES-originalerne. De er primært tooling, stier og kommandoer og er derfor i praksis sproguafhængige.

## Hvad bliver bevidst på engelsk?

Bevidst ikke oversat, fordi det er standard tech-vokabular:

- `cv.md`, `pipeline`, `tracker`, `report`, `score`, `archetype`, `proof point`
- Tool-navne (`Browser/CloakBrowser`, `WebSearch`, `WebFetch`, `Read`, `Write`, `Edit`, `Bash`)
- Statusværdier i trackeren (`Evaluated`, `Applied`, `Interview`, `Offer`, `Rejected`)
- Kodeblokke, stier og kommandoer

Målet er naturligt tech-dansk: dansk løbende tekst, engelske fagtermer hvor de faktisk bruges i danske teams.

## Ordliste

| Engelsk | Dansk i denne codebase |
|---------|------------------------|
| Job posting | Jobopslag / stillingsopslag |
| Application | Ansøgning |
| Cover letter | Ansøgning / motiveret tekst |
| Resume / CV | CV |
| Salary | Løn |
| Compensation | Lønpakke / samlet pakke |
| Skills | Kompetencer |
| Interview | Samtale |
| Hiring manager | Ansættende leder / hiring manager |
| Recruiter | Recruiter |
| AI | AI / kunstig intelligens |
| Requirements | Krav |
| Notice period | Opsigelsesvarsel |
| Probation | Prøvetid |
| Vacation | Ferie |
| Permanent employment | Fastansættelse |
| Fixed-term employment | Tidsbegrænset ansættelse |
| Collective agreement | Overenskomst |
| Pension scheme | Pension |
| Holiday allowance | Feriepenge / ferietillæg |

## Bidrag

Hvis du vil forbedre oversættelsen eller tilføje flere danske modes:

1. Opret et issue med forslaget
2. Hold samme tone og ordvalg som ovenfor
3. Oversæt idiomatisk, ikke ord-for-ord
4. Bevar strukturen i blokke, tabeller og tool-instruktioner
5. Test med et rigtigt dansk jobopslag før PR
