# SlopAudit Verification Methodology v1

Purpose: decide, with documented evidence, whether a YouTube channel is a mass-produced
AI content farm ("slop") or human-led content. This methodology is our IP and our defense:
every listing must survive a correction request.

## Classification outcomes

- **SLOP** — listed on the exclusion list. Mass-produced synthetic content, minimal human creative input.
- **HYBRID** — NOT listed. Human-led but AI-assisted. We never penalize disclosed, human-led AI use.
- **HUMAN** — NOT listed.
- **INSUFFICIENT** — NOT listed. We only list with evidence. When in doubt, leave it out.

## Signal battery (per channel)

### Tier 1 — volume forensics (strongest signals, cheap to check)
1. Upload cadence: >2 produced long-form videos/day sustained over 30+ days, or >8 Shorts/day.
2. Cadence vs. age: channel under 12 months with 500+ videos.
3. Output uniformity: video lengths clustered within ±10% (template pipeline marker).

### Tier 2 — template detection
4. Title structure: same syntactic template with swapped nouns across 20+ videos.
5. Script recycling: identical phrasing/beats across "different" videos.
6. Thumbnail assembly-line: same composition, AI-image artifacts (hands, text, lighting).
7. Description boilerplate: identical descriptions, often with the same hashtag block.

### Tier 3 — synthetic markers
8. TTS narration: flat prosody, no breaths/corrections, mispronounced proper nouns repeated identically.
9. AI visuals: Midjourney/SDXL artifacts, physically impossible scenes presented as real.
10. Zero human evidence: no face, no hands, no location shots, no livestreams, no community
    interaction beyond bot-like replies, across the entire catalog.

### Tier 4 — network markers
11. Cross-channel cloning: same template/voice across multiple "different" channels (slop networks).
12. Channel pivots: dormant or repurposed channel that flipped niche overnight to high-volume output.

## Listing threshold

List as SLOP only if: **≥2 Tier-1 signals AND ≥2 signals from Tiers 2–4**, documented with
specific video URLs/observations in the evidence file. One analyst review minimum (me),
spot-check sample re-reviewed before each list release.

## Evidence record format (per listed channel)

```
channel_id, handle, checked_date, tier1_signals, tier2_4_signals, evidence_notes, example_video_urls, reviewer, confidence (high/med)
```

Only "high" confidence ships to the public/free list. "Medium" stays internal for audit context.

## Corrections policy (public)

Anyone may dispute a listing with evidence of human-led production (BTS, livestream, process video).
Disputes reviewed within 72h. Wrongful listings removed immediately and logged publicly.
We sell placement hygiene, not accusations — the list's value IS its accuracy.

## Sources policy

Third-party blocklists (AiSList CC BY-NC, surasshu, press coverage) are used as LEADS ONLY.
Nothing enters our list without our own independent verification and evidence record.
We never bulk-copy: respects licenses, and our value is verification, not aggregation.

## Tooling note (for Claude)

With a free YouTube Data API key (10k units/day): channels.list + playlistItems.list + videos.list
≈ 3–5 units per channel → ~2,000 channel checks/day within free quota for Tier-1 signals.
Tier 2–3 require human/Claude review of actual content — budget ~15 verified channels/session.
