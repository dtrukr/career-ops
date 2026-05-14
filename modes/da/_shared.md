# Delt kontekst -- career-ops (Dansk)

<!-- ============================================================
     TILPASNING AF DENNE FIL
     ============================================================
     Denne fil indeholder delt kontekst for de danske career-ops-modes.
     Før brug skal du:
     1. udfylde config/profile.yml
     2. oprette cv.md i projektroden
     3. evt. oprette article-digest.md med proof points
     4. tilpasse sektioner markeret med [TILPAS]
     ============================================================ -->

## Kilder til sandhed (læses altid før vurdering)

| Fil | Sti | Hvornår |
|-----|-----|---------|
| cv.md | `cv.md` | ALTID |
| article-digest.md | `article-digest.md` (hvis den findes) | ALTID |
| profile.yml | `config/profile.yml` | ALTID |

**REGEL:** Opfind aldrig metrics eller proof points. Læs dem fra `cv.md` og `article-digest.md`.
**REGEL:** Hvis tal findes begge steder, vinder `article-digest.md`.

---

## North Star -- målroller

Behandl alle målroller seriøst. Ingen rolle er "sekundær", hvis løn, udvikling og match er gode.

| Arketype | Tematiske akser | Hvad de køber |
|----------|------------------|---------------|
| **AI Platform / LLMOps Engineer** | Evaluation, observability, reliability, pipelines | En person, der får AI i produktion med målbare signaler |
| **Agentic Workflows / Automation** | HITL, tooling, orchestration, multi-agent | En person, der bygger robuste agentsystemer |
| **Technical AI Product Manager** | GenAI/agents, PRDs, discovery, delivery | En person, der oversætter forretning til AI-produkt |
| **AI Solutions Architect** | Hyperautomation, enterprise, integrations | En person, der designer end-to-end AI-arkitektur |
| **AI Forward Deployed Engineer** | Kunde-nær levering, prototyping, tempo | En person, der leverer AI-løsninger hurtigt hos kunden |
| **AI Transformation Lead** | Change management, adoption, enablement | En person, der driver AI-transformation i organisationer |

### Adaptiv framing pr. arketype

| Hvis rollen er... | Fremhæv hos kandidaten... | Kilder til proof points |
|-------------------|---------------------------|--------------------------|
| Platform / LLMOps | Produktion, observability, evals, reliability | article-digest.md + cv.md |
| Agentic / Automation | Multi-agent, HITL, orchestration, error handling | article-digest.md + cv.md |
| Technical AI PM | Discovery, metrics, PRDs, stakeholder management | cv.md + article-digest.md |
| Solutions Architect | Systemdesign, integrationer, enterprise-parathed | article-digest.md + cv.md |
| Forward Deployed Engineer | Hurtig levering, kundevendt arbejde, prototype til drift | cv.md + article-digest.md |
| AI Transformation Lead | Adoption, enablement, organisatorisk forandring | cv.md + article-digest.md |

### Exit-fortælling

Brug kandidatens exit story fra `config/profile.yml` i ALT kandidatvendt materiale:
- I PDF-summaries
- I STAR-historier
- I ansøgningssvar og motivationsfelter

### Tværgående fordel

Frame profilen som **"teknisk builder med dokumenterbar praksis"**:
- Ikke en generalist uden dybde
- Ikke en ren strategist uden leverancer
- En person der kan bevise output med konkrete cases

### Portfolio / demo

Hvis kandidaten har en demo eller et dashboard i `profile.yml`, så tilbyd det i relevante ansøgninger.

### Lønintelligens

**Generelle regler:**
- Brug WebSearch til aktuelle markedsdata
- Frame efter jobtitel, ikke efter enkelte skills
- Konsulentrater ligger typisk tydeligt over fastansatte lønniveauer

### Dansk marked -- vigtige begreber

I danske jobopslag og kontrakter dukker disse begreber ofte op. De skal vurderes korrekt:

| Begreb | Betydning | Effekt på vurdering |
|--------|-----------|---------------------|
| **Overenskomst** | Kollektiv aftale om løn- og ansættelsesvilkår | Mindre forhandlingsrum, men mere forudsigelighed |
| **Pension** | Arbejdsgiverbetalt pensionsbidrag, ofte oven i grundlønnen | Skal tælles med i den samlede pakke |
| **Feriepenge / ferietillæg** | Lovbestemt eller kontraktuel feriekompensation | Må ikke glemmes i sammenligning af pakker |
| **Prøvetid** | Typisk de første måneder med kortere opsigelsesvarsel | Normalt markedsstandard, ikke automatisk rødt flag |
| **Opsigelsesvarsel** | Varsel ved opsigelse | Vigtigt for realistisk startdato |
| **Fastansættelse** | Permanent ansættelse | Lavere risiko end kontrakt/freelance |
| **Tidsbegrænset ansættelse** | Ansættelse med slutdato | Mere risiko, bør afspejles i score |
| **Fritvalgskonto** | Ekstra procentsats/valgbar pulje i nogle overenskomster | Lille men reel del af den samlede pakke |

### Forhandlingsscripts

**Lønforventning:**
> "Baseret på markedet for denne type rolle går jeg efter [RANGE fra profile.yml]. Jeg er fleksibel på strukturen, så længe den samlede pakke og rollen hænger sammen."

**Hvis de presser på geografisk rabat:**
> "De roller jeg er konkurrencedygtig til er output-drevne, ikke postnummer-drevne. Min dokumenterede effekt ændrer sig ikke med geografien."

**Hvis tilbuddet ligger under målet:**
> "Jeg sammenligner med muligheder i den højere ende af markedet. Jeg er interesseret i [company] på grund af [reason]. Kan vi udforske en pakke tættere på [target]?"

### Lokationspolitik

**I formularer:**
- Følg den faktiske tilgængelighed i `profile.yml`
- Skriv eksplicit om tidszone-overlap og hybridvillighed, når der er fritekst

**I vurderinger:**
- Hybrid uden for hjemlandet men stadig realistisk: score **3.0**, ikke 1.0
- Kun score 1.0 hvis opslaget kræver 4-5 dage on-site uden fleksibilitet

### Time-to-offer prioritet

- Hurtig, god nok ansøgning slår perfekt men forsinket ansøgning
- Demo + proof points > generiske bullets
- Brug 80/20

---

## Globale regler

### ALDRIG

1. Opfind erfaring, titler eller tal
2. Ændr `cv.md` eller portfoliofiler direkte
3. Indsend ansøgninger på kandidatens vegne
4. Del telefonnummer i genererede outreach-beskeder
5. Anbefal løn klart under markedet
6. Generér PDF uden først at have læst opslaget
7. Skriv corporate fluff
8. Ignorér trackeren

### ALTID

0. Hvis formularen tillader det, så lever et målrettet ansøgningsbrev eller en kort motiveret tekst
1. Læs `cv.md` og `article-digest.md` før vurdering
2. Kør `node cv-sync-check.mjs` ved første vurdering i sessionen
3. Detektér arketype og tilpas framing
4. Brug eksakte linjer fra CV'et i matching
5. Brug WebSearch til løn- og virksomhedsdata
6. Skriv på sproget i opslaget
7. Vær direkte og konkret
8. Når du skriver dansk: naturligt tech-dansk, korte sætninger, aktive verber
9. Nye tracker-poster som TSV i `batch/tracker-additions/`, ikke direkte i `applications.md`
10. Hver rapport skal have `**URL:**` i headeren

### Tools

| Tool | Brug |
|------|------|
| WebSearch | Løn, marked, kultur, kontakter, fallback for opslag |
| WebFetch | Statiske opslag og fallback |
| Browser/CloakBrowser | Aktive opslag, SPAs, live læsning af karrieresider |
| Read | `cv.md`, `article-digest.md`, `cv-template.html` |
| Write | Midlertidig HTML, reports, tracker-relaterede filer |
| Edit | Opdatering af eksisterende tracker-data |
| Bash | `node generate-pdf.mjs` og hjælpe-scripts |
