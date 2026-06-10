# SlopAudit — Outreach Kit

Daily rhythm: 10 emails/day, sent from your normal Gmail, person-to-person.
No bulk tools, no sequences — at this volume, deliverability is fine and replies are human.

---

## Who we email (in priority order)

1. **Small PPC / performance-marketing agencies** (2–20 people) running YouTube/Performance Max for clients.
   Why: they manage many accounts → one yes = recurring audits across their book of clients.
2. **D2C brand marketing managers** spending $5k–100k/mo on Google Ads.
3. **Freelance Google Ads consultants** (they buy tools that make them look good to clients).

How I (Claude) find them each session: web research for agencies' public contact emails
(their own sites' contact pages — public business addresses, not scraped personal data).
You bring me back 30 minutes; I hand you 10 names + personalized first lines.

---

## Email template A — the free-sample open (primary)

Subject: `your clients' YouTube placements (quick flag)`

> Hi {{FirstName}},
>
> Quick context: YouTube purged 16 AI-slop networks in January (4.7B views) — but the purge only
> caught the biggest. Kapwing measured that 20%+ of Shorts shown to new users is still AI slop,
> and Google Ads keeps serving placements on these channels. Most accounts we look at are paying
> for some of it.
>
> I run SlopAudit — we screen YouTube placement reports against a human-verified database of
> AI-slop channels and send back a ready-to-upload exclusion file.
>
> If you send me any account's placement report export (2 clicks in Google Ads), I'll screen the
> top 200 placements free and send back what we flag, within 48h. No call, no pitch deck.
>
> Worst case you confirm your accounts are clean.
>
> — Revanth, SlopAudit
> {{SITE_URL}}

## Email template B — the data hook (for agencies with blogs/newsletters)

Subject: `data: how much of YouTube ad spend hits AI slop?`

> Hi {{FirstName}},
>
> I'm building the public dataset of verified AI-slop YouTube channels (the community lists are
> consumer-side; nothing exists formatted for Google Ads exclusions).
>
> We're publishing a monthly report on slop placements — first edition includes anonymized stats
> from audited accounts. Want your agency's accounts in the baseline (free, anonymized)? You get
> the flagged placements back before anyone else sees the aggregate.
>
> — Revanth

## Follow-up (one only, +4 days, reply in same thread)

> Hi {{FirstName}} — closing the loop. If placement hygiene isn't on your plate this quarter, no
> worries at all. If it is: free screen of your top 200 placements stands. 48h turnaround.

Rules: never a third email. Every reply gets answered within 24h (paste them to me).

---

## The audit workflow (what happens when someone says yes)

1. They export: Google Ads → Insights & reports → When and where ads showed → YouTube placements → Download CSV.
2. You forward the CSV to me here.
3. I screen every placement: volume forensics, template detection, synthetic markers (see METHODOLOGY.md).
4. I return to you, you send to them:
   - `flagged_channels.csv` (with evidence notes per channel)
   - `exclusion_upload.csv` (Google Ads placement-exclusion format)
   - 5-line summary: X placements screened, Y flagged, ~Z% of impressions affected
5. Free mini-audit → offer full audit $99 → after 2 paid audits, offer monthly monitoring (recurring).

## Metrics that decide things (be honest with ourselves)

- 100 emails sent → expect 2–5 replies, 1–3 free audits. Below that: template/test problem, I rewrite.
- 3 free audits delivered → expect ≥1 paid conversion. Zero conversions after 5 free audits = pricing or pain problem, we reassess.
- Kill criterion: 200 emails + 0 audits requested = the channel is dead, we pivot the offer (not the dataset).
