# The Selah Yiddish Rendering — NOTES

*yi.v1 · chair 69 · seated 2026-09-11 (Rosh Hashanah 5787). The first
chair that shares the source's script — the Name stands at its seat as
יהוה itself, in its own letters, in a language whose tradition would
have hidden it.*

## The seal

| Count | Value |
|---|---|
| Verses | 23,213 / 23,213 |
| Token spine ≡ en floor | 23,213 / 23,213, zero mismatches; surface parity zero |
| יהוה at the Name seat | **6,828 / 6,828 — and 6,828 in the flow. Exact.** The identity chair: seat glyphs ≡ flow glyphs |
| אלהים (flow) | 2,304 |
| ⟨את⟩ | 11,866 in the token row ≡ 11,866 in the flow ≡ the en floor, per-file 0 off |
| Erasure (ה׳ / השם / אדושם / אלוקים / יי־ligature / דער אויבערשטער / ג־ט / הקב״ה) | **0** at every Name seat (the one השם is the Gizonite's own name, 1 Chr 11:34 — lawful) |
| גאָט at a Name seat | **0** (16 verses carry it — all foreign gods or גאָט־פֿאַרכטיק for ירא אלהים) |
| German thermometer (אונד / ניכט / איסט) | **0 · 0 · 0** |
| גיהנום for Sheol | **0** — Sheol stands as שאול inline |
| ⟨ית⟩ | **0** corpus-wide |
| Aleph-tav audit | `[]` — defective 0, misaligned 0 |
| Empty glosses | 5 — the en floor's own five lawful holes, mirrored exactly |
| Latin script in flow or gloss | **0** |

## Cruxes of the chair

- **The identity held.** Tekoa's headline: the one risk the shared
  script creates — that the Name gets absorbed into the language's own
  avoidance apparatus — *did not happen*. All 6,828 seats gloss יהוה
  unpointed and unsubstituted; after seating repairs the flow count is
  exactly 6,828 too (five surplus-Name flows repaired: duplicated
  clauses at 2 Sam 6:9 and Jer 44:21, supplied subjects at Prov 15:9
  and 1 Chr 5:41, and Isa 30:18's אלהי משפט mis-carried as the Name).
- **Points are letters.** Yiddish pointed letters (אַ אָ פּ פֿ בֿ תּ שׂ ייִ)
  are letters of the orthography, never stripped. The chair's
  characteristic bleed ran the other way: WLC vocalization traveled
  with inline loshn-koydesh into the flow — 1,509 Hebrew-only marks
  (te'amim included, some spliced mid-word into Yiddish) stripped by a
  whitelist cleaner (`dev/scripts/yi_tekoa_class_a.py`) that preserves
  the seven Yiddish points. **A generic "strip niqqud" is itself the
  danger on this chair.** Token surfaces stay bare-consonantal per the
  en floor.
- **The suffixed-את discipline.** 157 gloss seats carried wrapped
  forms (⟨אתו⟩, ⟨אתכם⟩ …) invisible to the counters; all rewritten to
  bare ⟨את⟩ + Yiddish pronoun per the qu-seal rule, and 109 leftover
  flow wraps adjudicated seat-by-seat against the actual Hebrew את
  positions — 55 flows hand-seated (including the נשיאים splice at
  Josh 13:21, where an auto-insert had landed inside the word).
- **Dan 3:12, the sixteenth chair.** יתהון is the Aramaic pronoun
  object, not the marker: bare זיי, no ⟨את⟩, no ⟨ית⟩, per every sibling.
- **The re-press.** 24 verses re-rendered at seating: 4 flows that
  dropped the Name (Isa 49:25, Jer 26:16, Nah 1:2, Zech 1:16 — highest
  severity on an identity chair), 4 raw pointed-Hebrew flows
  (Prov 23:13–16), 8 wrong-language flows (2 Kgs 20:1–4 in English;
  Ezek 11:15 and Hos 13:13–15 in romanized Yiddish — the script-home
  ruling: romanization never wins v1), 5 truncations, plus partials.
- **The German bleed showed as script-switching, not vocabulary.**
  Thermometer at absolute zero, but 93 Latin fragments welded mid-word
  (פֿאַרchten, באַזmurderדיקטע, גewicht) — every weld repaired to its
  evident Yiddish word.
- **Hebrew-inline posture.** 4.8% of flow words are loshn-koydesh
  standing in the source's own spelling (מזבח, ברית, כהן, נפֿש, תּורה) —
  normal, idiomatic Yiddish, not untranslation. ערד/לאַנד split for ארץ
  filed as Class B.

## Tekoa

Verdict: **SEATS** — "the alignment spine is the cleanest of any chair
I have inspected." Full report:
`data/experiments/yi-seating/yi-tekoa-report.md` (selah repo).
Class A applied in full at seating (~2,000 field edits across ~700
files). Class B filed PENDING SCOTT, headline items: B1 הבל → הויך
(defensible — *hoykh* < *Hauch*, breath — but homographic with
*high*); B2 488 unpointed-*ksiv* verses (both orthographies lawful);
B5 supplied-word ⟨…⟩ marking 48× lighter than the floor; B9 Prov 8:22
קנני *created* vs floor *possessed*.

## The burn

23,213 / 23,213 verses, z.ai glm-5.3 (tier lane glm-5.2, one verse
pressed through the glm-5.3 tier), burned 2026-09-10, seated
2026-09-11. Ladder for stragglers: max-tokens 24–32k first, then
temp 0.55, then the glm-5.3 tier — never the model before the ceiling.
Rails: `docs/methodology/translation-discipline/yi.md` (written in
Yiddish), benched 2d8777e0.
