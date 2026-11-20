# BUILD_LOG — news-image-20261120 (hybrid: v1 legibility + v2 breadth)

Built 2026-11-20 in this builder session (side chat "News Image
20261120", opened by the user's first message "lanjut"). All files
written fresh in this session; `main.ts` was not copied from the
19 Nov entry (read only as a reference for the PNG-encoding
technique). No push, bundle or submit done here — parent verifies,
pushes, submits.

## Kit facts

- Competition: `news-image-20261120` — "Sum up 20 November's world
  news in one image". Opens 2026-11-20T00:00:00Z, deadline
  **2026-11-22T00:00:00Z (07:00 WIB 22 Nov)**.
- Prize: **$250** total, top 50 paid: 1st $50, 2nd $30, 3rd $15,
  4th–10th $5, 11th–50th $3. Final heat: 3 Swiss rounds + playoff
  of top 52; AI judge (z-ai/glm-5.3-flash) compares images pairwise,
  no news feed, criteria in order: (1) names the day + specific
  events of that day (not before 13 Nov 2026), (2) selection/breadth
  across regions and fields, (3) reads from the image alone,
  (4) faithful, no hype/speculation as fact, (5) craft, legible at
  ~300 px across.
- Output: program writes ONE image to `/output/entry.png` — PNG or
  JPEG, at most 1 MiB, at most 1024x1024. Program: Node 22 `main.ts`
  (or Python 3.13), stdlib only, no network, runs twice, both runs
  byte-identical. 60 s, 1 CPU, 512 MB.
- Submission limits: at most 10/day and 20 total (Force_Last).
  Quota checked by parent before build: can_submit yes, 3/3 left
  today, hard limit 20/20, 0 entries made in this competition.
- Kit: `~/workspace/makefun/news-image-20261120-kit/` (bundle_sha256
  `63afd6ef327953b503d6a89b46620965d4844234f8456ecdcec384c86d63f66e`).

## Lessons applied from 19 Nov (v1 rate 0.970769, v2 0.964993,
## top-50 line 0.987638)

- v1: clean layout, only 6 stories — too few. v2: 19 stories in a
  dense 3x6 grid — text shrank unreadably at thumbnail size and
  scored WORSE than v1. Density for its own sake hurts.
- This entry: hybrid — v1's clean masthead + lead story, 11 further
  stories in a 3x4 grid (cell 317x140, much roomier than v2's
  317x96), 12 stories total + footer ticker. Headline max 2 lines,
  summary max 1 line, self-check throws on overflow.

## Stories chosen (all reporting dated 20 Nov 2026)

1. **Lead — Russia hits three Kyiv bridges (overnight 19→20 Nov).**
   Ballistic missiles hit the Podilsko-Voskresenskyi, Darnytskyi
   and Pivdennyi bridges over the Dnipro; 3 killed, 15 injured;
   biggest strikes on the capital's crossings since the war began;
   retaliation for Ukraine's three attacks on the Crimean Bridge
   that week. Sources: Reuters ("Three killed in missile strikes
   on Kyiv, mayor says, in biggest attack on bridges", 20 Nov),
   AP ("Russian attacks on Kyiv kill 3, cripple bridges and cut
   power", 20 Nov).
2. **Shenzhen peace declaration falls flat (20 Nov reaction).**
   Europe dismisses the Trump–Xi–Putin "peace declaration" as a
   "photo op"; Zelensky says Ukraine accepts no deals made without
   Kyiv; coalition of the willing gathers in Berlin. The summit
   itself was 19 Nov — carried here ONLY as its 20 Nov reaction,
   never as a 20 Nov event. Sources: The Times ("Your Putin
   meeting changes nothing for Ukraine, Europe tells Trump",
   20 Nov; "Trump, Xi and Putin pledge to reform UN and boost oil
   production", 20 Nov), Reuters ("Trump's personalized diplomacy
   hits its limits with 3-way summit", 20 Nov).
3. **COP31 endgame, no deal (Antalya, 20 Nov).** Final scheduled
   day; revised draft drops every mention of fossil fuels;
   negotiators divided, talks may spill past Friday's close.
   Sources: Reuters ("COP31 negotiators publish revised deal text
   with no mention of fossil fuels", 19–20 Nov), phys.org ("UN
   climate talks enter crunch time with no deal in sight",
   20 Nov).
4. **Cyclone Akvan makes landfall (Odisha, 20 Nov).** Crossed the
   north Andhra Pradesh–south Odisha coast near Gopalpur Fri
   morning, 70–80 kmph gusting 90; 300,000+ evacuated; no major
   damage or loss of life reported so far; third cyclone to hit
   India in under a month. Sources: Reuters ("India's eastern
   coast hit by third cyclone within a month", 20 Nov), IMD via
   The Hindu BusinessLine live blog (20 Nov).
5. **UK–EU youth mobility deal (Brussels summit, 20 Nov).**
   Up to 100,000 visas a year in each direction, ages 18–31, stays
   up to 3 years; centrepiece of the Brexit reset. Sources: BBC
   ("UK and EU to agree youth mobility scheme", 20 Nov), The Times
   ("Andy Burnham agrees to 100,000 visas in EU youth mobility
   scheme", 20 Nov).
6. **Houthi missile hits Riyadh's PIF Tower (reported 20 Nov).**
   Strike on Thursday damaged windows across 7–8 floors of the
   80-storey tower housing the Saudi sovereign wealth fund HQ; no
   injuries; second hit on the financial district in two weeks.
   Worded as the Friday reporting of it. Sources: Reuters via
   Devdiscourse ("Riyadh's tallest skyscraper hit in Houthi
   strike", 20 Nov 00:57 IST), WSJ ("Houthi Attack Damages Saudi
   Capital's Tallest Tower", 20 Nov).
7. **Anthropic soars on Nasdaq debut (reported 20 Nov).** Shares
   opened at $111.50 (+34% on the $83 IPO price), briefly valued
   the firm near $2tn, closed at $97.17 (+17%) — biggest IPO in
   history at $81.3bn. Trading was Thursday; carried as the Friday
   reporting of the debut close. Sources: Reuters ("Anthropic's
   $1.5 trillion debut rewrites venture capital's playbook",
   20 Nov), WSJ ("Anthropic Opens Up 34% at $111.50 a Share",
   20 Nov).
8. **Unknown objects fall near Poland's Ukraine border (20 Nov).**
   Polish army investigates two possible airspace violations after
   Russia's overnight attack; jets scrambled, alerts lifted by
   07:30; PM Tusk: no current air threat. Sources: Reuters
   ("Polish army investigates report of unknown objects near
   Ukraine border", 20 Nov).
9. **Tankers hit mines off Hormuz, ablaze (reported 20 Nov).**
   Iran's navy/army says two (army: three) tankers caught fire
   after striking naval mines in a restricted area east of the
   Strait of Hormuz; claims not independently verified. Worded
   "IRAN REPORTS TWO ON FIRE". Sources: Reuters ("Oil prices edge
   higher as Houthi attacks on Riyadh raise supply concerns",
   20 Nov), Middle East Eye via hathalyoum (20 Nov).
10. **Rohingya welcome the ICJ verdict (20 Nov reaction).**
    Refugees in Bangladesh welcome the court's genocide ruling
    against Myanmar but say they want to go home. The ruling
    itself was 19 Nov — carried here ONLY as the 20 Nov reaction.
    Source: Toronto Star ("Rohingya in Bangladesh welcome UN
    court's genocide verdict but say they want to go home",
    20 Nov).
11. **Nigeria moves to end jail terms for attempted suicide
    (20 Nov).** Source: BBC via Jabulani Radio top-stories roundup
    (20 Nov).
12. **M5.6 quake southeast of the Loyalty Islands (20 Nov,
    00:49 UTC).** Shallow (10 km), offshore New Caledonia; no
    tsunami threat, no damage reported. Source: USGS via
    watchers.live / terremoto (20 Nov).
13. **Footer ticker:** Genoa airport suspends flights after
    unidentified drones detected (Daily Baku, 20 Nov); Japan core
    inflation 2.2% in October, highest this year as energy
    subsidies end (Daily Brief, 20 Nov).

Dropped as not cleanly 20 Nov: US loses measles elimination status
(PAHO announced 17 Nov); Trump pardons Pete Rose (announced Thu
19 Nov); US Senate rejects Iran war-powers resolution 51–48
(19 Nov evening); ICJ Rohingya ruling itself (19 Nov — only the
reaction is used); Shenzhen summit itself (19 Nov — only the
reaction is used); Anthropic IPO pricing (19 Nov — only the debut
close as reported 20 Nov is used).

## Files written (all fresh in this session)

- `main.ts` — Node 22, stdlib only (`node:fs`, `node:path`,
  `node:zlib`). Hand-written PNG encoder (CRC32 + deflate level 9),
  5x7 bitmap font stored as strings, flat vector drawing (bridge
  over the Dnipro with blast + smoke for the lead). No network, no
  clock, no randomness. Layout: masthead (date + story count), lead
  story with bridge art, 3x4 grid of 11 story cells + sources box
  (tag, headline ≤2 lines, summary ≤1 line), footer ticker.
  Self-checks throw if the lead headline wraps past 2 lines, the
  lead summary past 2, any cell headline past 2 lines, or any cell
  summary past 1 line.
- `README.md` — entry description, story list, run instructions.
- `LICENSE` — MIT, first line `SPDX-License-Identifier: MIT`.
- This `BUILD_LOG.md`.
- No `.makefun/owner.json` (parent adds it). No GitHub repo
  created, nothing pushed or submitted here.

## Verification

- 2x run (after final fix): `MAKEFUN_OUTPUT_DIR=/tmp/ni20-out1
  node main.ts` and `/tmp/ni20-out2` → **byte-identical**, sha256
  `8f8a79913765e31006e95a7f86effd169f790ad0ee8770440e1c50dd2af49b19`
  (first version before the lead-spacing fix:
  `bb56d1ed596ff39315714f7615c65ec49d7ee58c07747a20548ef7bd6c30cd78`).
- Output: **1024x1024 RGB PNG, 21,161 bytes** (< 1 MiB,
  ≤1024x1024). PNG chunks validated with Python (IHDR/IDAT/IEND,
  all CRCs ok, bit depth 8, colour type 2).
- Node 22 note: `main.ts` uses no TypeScript-only syntax (plain JS
  in a `.ts` file), so it runs under Node 22 type stripping as well
  as Node 24 used locally (v24.22.1).

## Visual inspection (actual output image, viewed directly)

- Full size (1024x1024): masthead + date legible; lead headline
  2 lines, bridge art + blast + smoke clean; all 11 grid cells
  complete, no overlap, no cut-off text; sources box and footer
  ticker legible. One fix made after the first viewing: the lead
  summary's second line ("STRIKES.") overlapped the SOURCES line
  — summary moved from y 236 to y 230 and sources from y 276 to
  y 278, then re-ran 2x and re-viewed; overlap gone.
- At ~300 px (downscaled and viewed): masthead, date and lead
  headline still read clearly; cell headlines are small but
  decipherable as blocks, tags and one-line summaries blur — the
  expected cost of a grid, and better than v2's 3x6 (cells here
  are 140 px tall vs v2's 96). Headlines carry each story at
  thumbnail size.

## Remaining risks

- Judge is a VLM with no news feed: it judges from the image + its
  own knowledge. Three cells (Riyadh PIF tower, Anthropic debut,
  Hormuz tankers) report Thursday events first widely reported on
  Friday; they are worded as the Friday reporting, and the rules
  allow "first reported" on the day, but a judge that dates them
  to Thursday could count them as yesterday's news — bounded to
  3 of 12 stories. The Shenzhen summit and ICJ ruling appear only
  as Friday reactions, not as Friday events.
- The build was made Friday afternoon WIB (~17:30), when the day
  was only half over in the West — no Friday US market close or
  late-European outcomes could be included. A rival built later
  in the day may carry more of Friday.
- Dev rate is provisional and opponent-adjusted: v1 went 12-0 yet
  rated only 0.970769. Top-50 paid line for 19 Nov was 0.987638;
  this entry is a long shot, as v1/v2 were.
