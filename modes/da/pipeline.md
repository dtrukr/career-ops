# Mode: pipeline -- URL-indbakke (second brain)

Behandler URLs til jobopslag, som er samlet i `data/pipeline.md`. Kandidaten kan gemme links løbende og senere køre `/career-ops pipeline` for at behandle dem samlet.

## Workflow

1. Læs `data/pipeline.md` og find alle `- [ ]` under "Pending", "Pendientes", "Offen" eller tilsvarende
2. For hver åben URL:
   a. beregn næste `REPORT_NUM`
   b. udtræk jobopslaget med browser/CloakBrowser -> WebFetch -> WebSearch
   c. hvis URL'en fejler, markér den `- [!]` og fortsæt
   d. kør fuld auto-pipeline: vurdering -> rapport -> PDF (hvis relevant) -> tracker
   e. flyt posten til den færdige sektion som `- [x]`
3. Ved 3+ åbne URLs: kør flere agenter parallelt
4. Afslut med en kort tabel:

```markdown
| # | Virksomhed | Rolle | Score | PDF | Anbefalet handling |
```

## Format af pipeline.md

```markdown
## Pending
- [ ] https://jobs.example.com/posting/123
- [ ] https://job-boards.greenhouse.io/company/jobs/456 | Company ApS | Senior PM
- [!] https://private.url/job -- fejl: login kræves

## Processed
- [x] #143 | https://jobs.example.com/posting/789 | Acme | AI PM | 4.2/5 | PDF ✅
```

## Smart udtræk fra URL

1. **Browser/CloakBrowser først** for SPAs og moderne ATS'er
2. **WebFetch** som fallback til statiske sider
3. **WebSearch** som sidste udvej

**Danske specialtilfælde:**
- **Jobindex**: godt til discovery, men læs helst det oprindelige opslag før endelig vurdering
- **The Hub**: stærk til nordiske startups
- **Work in Denmark**: nyttig til engelske roller og internationale ansættelser
- **Jobnet**: kan kræve login; markér som `[!]` hvis opslaget ikke er offentligt tilgængeligt

## Automatisk nummerering

1. List filer i `reports/`
2. Find højeste eksisterende præfiks
3. Brug næste nummer

## Synk af kilder

Før behandling af nogen URL:

```bash
node cv-sync-check.mjs
```

Advar kandidaten hvis CV, profil og proof points ikke hænger sammen.
