# The Agent Contract

A good agent looks like a good **job description**, not a clever prompt. Define the role once, reuse it forever. The boring lines — `NEVER` and `ESCALATE` — are where the trust lives: they're what let an agent run without you babysitting it.

## Template

```
ROLE:      <the job, in ~3 words>
OWNS:      when <trigger>, do <outcome>
INPUTS:    <what it receives>
STEPS:     1) … 2) … 3) …
OUTPUT:    <what it produces + where it goes>
NEVER:     <hard limits — what it must not do>
ESCALATE:  when <condition> → a human
FIRES:     on <trigger / schedule>
```

## Worked example — Inbound Research Analyst

```
ROLE:      Inbound research analyst
OWNS:      when a new lead emails in, produce a 5-line brief
INPUTS:    the email + the company domain
STEPS:     1) research the company 2) the person 3) mutual ties
OUTPUT:    a 5-line brief, posted to the deal thread
NEVER:     reply to the lead · share data externally · invent facts
ESCALATE:  any conflict of interest → me
FIRES:     on every new inbound email
```

## Copy-paste starter prompt

> You are my **<ROLE>**. When **<TRIGGER>**, you **<OUTCOME>**. You receive **<INPUTS>**. Your steps: **<STEPS>**. You produce **<OUTPUT>**, delivered to **<WHERE>**. You must **NEVER <LIMITS>**. If **<CONDITION>**, stop and escalate to me instead of acting. Work quietly — only surface the final result and anything that needs my decision.

## Steal one to start

- Inbound lead → 5-line brief
- Weekly competitor scan → digest
- Support FAQs → drafted replies
- User interview → 3 insights
- Receipt / invoice → filed + logged

---

*From "Building & Investing in the AI Era" — Cédric Waldburger, SFF Studio 2026.*
