# Mode: tilbud -- Fuld vurdering A-F

Når kandidaten indsætter et jobopslag (tekst eller URL), lever ALTID alle 6 blokke.

## Trin 0 -- arketype-detektion

Kortlæg opslaget til én af de 6 arketyper i `_shared.md`. Hvis rollen er hybrid, angiv de to nærmeste.

## Blok A -- rolleopsummering

Lav en tabel med:
- Detekteret arketype
- Domæne
- Funktion
- Senioritet
- Remote/hybrid/on-site
- Teamstørrelse (hvis nævnt)
- TL;DR i én sætning

## Blok B -- match mod CV

Læs `cv.md`. Lav en tabel hvor hvert krav i opslaget mappes til eksakte linjer i CV'et.

For hvert gap:
1. Er det en hard blocker eller nice-to-have?
2. Findes der nærliggende erfaring?
3. Kan et proof point fra portfolio dække noget af hullet?
4. Foreslå en konkret mitigation til ansøgning eller samtale

## Blok C -- level og strategi

1. Detekteret level i opslaget vs kandidatens naturlige level
2. Hvordan kandidaten kan sælge sig senior uden at overdrive
3. Hvad der er acceptabelt hvis rollen er et halvt niveau lavere

## Blok D -- løn og efterspørgsel

Brug WebSearch til:
- Aktuel løn for rollen i Danmark
- Virksomhedens løn/arbejdsgiver-signaler
- Efterspørgsel på denne type rolle

Vis kilder i tabel. Hvis data mangler, så sig det åbent.

**Danmark -- tjek altid:**
- Pension nævnt?
- Feriepenge eller ferietillæg nævnt?
- Bonus, warrant-program eller aktier?
- Overenskomst?
- Fastansættelse vs tidsbegrænset / freelance?

## Blok E -- personaliseringsplan

| # | Sektion | Nu | Foreslået ændring | Hvorfor |
|---|---------|----|-------------------|---------|
| 1 | Summary | ... | ... | ... |

Top 5 ændringer til CV + top 5 ændringer til LinkedIn for at løfte matchet.

## Blok F -- samtaleplan

Lav 6-10 STAR+R-historier:

| # | JD-krav | STAR+R-historie | S | T | A | R | Reflection |
|---|---------|-----------------|---|---|---|---|------------|

Reflection-delen skal vise senioritet: hvad kandidaten lærte, eller hvad de ville gøre anderledes i dag.

Tag også med:
- 1 anbefalet case study at vise
- Relevante red-flag-spørgsmål og gode svar

---

## Efter vurderingen

### 1. Gem rapporten

Gem vurderingen i `reports/{###}-{company-slug}-{YYYY-MM-DD}.md`.

**Format:**

```markdown
# Vurdering: {Virksomhed} -- {Rolle}

**Dato:** {YYYY-MM-DD}
**Arketype:** {detekteret}
**Score:** {X/5}
**URL:** {jobopslagets URL}
**PDF:** {sti eller pending}

---

## A) Rolleopsummering
...
```

### 2. Registrér i trackeren

Registrér altid i `data/applications.md`:
- næste løbenummer
- dato
- virksomhed
- rolle
- score
- status `Evaluated`
- PDF `❌` eller `✅`
- link til rapporten

**Tracker-format:**

```markdown
| # | Date | Company | Role | Score | Status | PDF | Report |
```
