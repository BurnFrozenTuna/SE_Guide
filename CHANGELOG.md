# Changelog

## v2.8.2

- **StoryEngine Original lock period corrected: 90 days → 180 days.** The post-activation
  restriction window (no deleting, privating, disabling Original, or uploading elsewhere)
  is now 180 days. Updated in both the field description and the regional-confirmation
  note, both editions. Reported by a fellow creator.

## v2.8.1

- **Two "don't let names collide" tips.** Lorebook: pick distinctive trigger words, since
  literal matching means a common word misfires (from a fellow creator who hit this).
  Variables: keep names clearly distinct, since look-alike names can cross their values.
  Both editions.

## v2.8.0

- **Made the click-to-connect port behavior a general point, not a story-node aside.**
  Every node's input ports open a pick-list when clicked — image ports included — and this
  was previously only mentioned in a story-node caption, which made creators think it was
  story-node-only. Added a shared explanation and a screenshot (an image port opened to its
  node list) to the overview. Same image in both editions.

## v2.7.3

- (JA) **Native-speaker polish.** Reworded the awkward 操舵 ("steer") metaphor in the
  inner-thought tip to natural Japanese, and smoothed several sentences in the header and
  disclaimer (guide intro, node-reference eyebrow spacing, the "believe the Canvas" line).
  Thanks to fellow creators for the review.

## v2.7.2

- **Clarified what the Prologue Message actually does.** It isn't only the reader's opening
  screen — the AI reads it too and treats it as established opening context (who's present,
  what's in motion, whether a macro should fire on turn one). Also documented a common
  practical trick: since the Prologue Guide is only 300 tokens, creators seed first-turn
  overflow into the prologue message, which the AI reads anyway. Both editions.

## v2.7.1

- Added a tip box near the top linking to Tiktokenizer (o200k_base) for counting tokens
  before pasting, since the Canvas shows no live count while writing. Framed as a close
  estimate, not verified against the Canvas — StoryEngine creators were told the model is
  GPT-4o, whose tokenizer is o200k_base. Added to both editions.

## v2.7.0

- **Expanded the sub-model description.** Beyond Full Story retrieval, the sub-model also
  handles memory — summarising and managing the running conversation (the machinery the
  Info Management / Long-term Memory toggles switch off) — and is reportedly involved in
  variable management too. This side is easy to overlook and was a common stumbling
  point. Reported by a creator; the variable-management part is flagged as not fully
  confirmed. Applied to both editions.
- (JA) Annotated the first lorebook mention as ロアブック（マクロ） to tie the term to the
  in-product マクロプロンプト label.

## v2.6.1

- Fixed the language tabs and image paths in the Japanese edition, which used relative
  paths and could resolve to /ja/ja/ (404) or miss shared images. All switched to
  absolute /SE_Guide/... paths so they work from either page.

## v2.6.0

- **Added a Japanese edition (ja/index.html).** Full translation of the guide, reached
  via a language tab (English / 日本語) in the sidebar. UI labels use the actual
  in-product Japanese wording; Japanese UI screenshots are used where available, and the
  rest are shared with the English edition.

## v2.5.1

- **Thumbnail WebP limit raised to 5 MB** (from the old ~2–3 MB) per a mid-2026 platform
  update. Also noted the platform's caveat that high-file-size or multi-frame images may
  lose some quality in the shrunk main-screen thumbnail.

## v2.5.0

- **Added a multilingual invitation to the issue tracker.** Readers can open an issue in
  their own language (Korean, English, Japanese, or Spanish) and get a reply in that
  language; rough machine translation is welcome too. Added to both the guide's closing
  note and the README.

## v2.4.3

- Credited **Scoot** by name with a link to their page, which the previous entry was
  missing, and noted that the check was a creator-to-creator one rather than an
  official statement from the platform.

## v2.4.2

- **Established that the StoryEngine Original terms are region-independent.** The
  previous version flagged the KRW milestone figures as possibly KR-only.
  [Scoot](https://storyengine.live/c/scootster), a creator working in the
  English-language region, checked the panel on their own account and the wording came
  back identical. The uncertainty note is replaced with that finding, shared with their
  permission — thank you.

## v2.4.1

- **StoryChat Original is now StoryEngine Original, and its terms were overhauled.** The
  old percentage-point settlement bonus is gone, replaced by fixed milestone payouts
  (KRW 100,000 at 10,000 eligible chats, a further KRW 200,000 at 50,000). Added the new
  rules: activate before first upload or within 6 hours, 2 works per month, only
  post-activation chats count, and collaborators/revenue shares are frozen for 90 days.
- Added a regional caveat: those amounts are quoted in KRW and it is **not confirmed**
  that non-KR creators see the same figures.

## v2.4.0

- **Corrected the retrieval architecture.** The lorebook (macro) is **not** handled by the
  sub-model. It's a separate, rule-based path: keyword-matched and injected directly into
  the main context, with no model reworking it in between. The **sub-model handles only
  Full Story**, via semantic search. The "two models" section and the lorebook section
  were reworded to keep these two paths clearly apart.

## v2.3.2

- **Corrected the reader token budget.** It is **2,000 tokens shared between User Notes
  and User Persona**, not 1,000 for notes alone as previously written. Past 2,000, the
  usage fee rises 10% per additional 600 tokens. Worked example updated to 776 of 2,000.
  Reported by [ㅇㅅㅇㅇㄴㄷ](https://storyengine.live/c/osoond) — second correction from
  them, thank you.

## v2.3.1

- Corrected a conflation in the v2.3.0 tip. The **in-reply summary code block** (which
  the model prints because Core Context instructed it to) is **not** the **Status View
  node** (a separate side panel). Reworded to keep the two apart, and cross-linked both
  ways.

## v2.3.0

- **Added craft guidance on status view placement.** Because the status block renders
  inside the model's output and a model writes top to bottom, its position decides what
  it can draw on: placed at the bottom, values are derived from the prose above; placed
  at the top, the prose is written to match the figures.
- Documented that **inner-thought lines steer the next turn** rather than being purely
  decorative — whatever the character is left thinking becomes context for the following
  response.

## v2.2.4

- Added a real-canvas screenshot to the Achievement node section, showing four
  variable → trigger → achievement chains running in parallel. Variable names are
  blurred by the author.

## v2.2.3

- Fixed a unit typo: the Preset Notes **Prompt** limit is **500 tokens**, not 500 chars.

## v2.2.2

- Added an **author-side (canvas) screenshot** to the Preset Notes section, shown before
  the reader-side one, so both perspectives are covered. Prompt bodies in it are blurred
  by the author on purpose — a real tutorial build leaves them empty.

## v2.2.1

- Clarified the Preset Notes token cost: the reader's User Notes budget is **free only
  up to 1,000 tokens**, and paid beyond that. Enabling preset notes draws from that pool,
  so a heavy note can push the reader into paying. Added a worked example (368 + 408 =
  776 of the free 1,000).

## v2.2.0

- **Preset Notes promoted from a one-line card to a full section.** Documented the key
  behavior that was missing: enabling a preset note **spends the reader's User Notes
  token budget**, which is why not all 10 can run at once. Also noted preset input lands
  at the bottom of the priority order. Added a reader-side screenshot.

## v2.1.1

- **Removed the word "RAG" from the lorebook section.** The lorebook fires on **exact
  keyword matching**, not similarity/vector search, so calling it RAG was inaccurate.
  Reworded to describe the actual mechanism. The internal method behind Full Story
  remains undocumented and is left as such.

## v2.1.0

- **New section: Scenario branching.** Story nodes set to `Is Start: No` can be wired
  behind a trigger and used as branch destinations, giving a visual-novel style route
  select. Technique reported by [ㅇㅅㅇㅇㄴㄷ](https://storyengine.live/c/osoond) — thank you.
- Story node section now points to the branching section instead of asking for help
  working it out.

## v2.0.4

- Added a link to GitHub Issues in the closing note, so "corrections welcome" actually
  says where to send them.

## v2.0.3

- **Advanced Settings token bonuses measured for all eight toggles**, one at a time:
  Long-term Memory +1,200, Macro Prompts +1,200, Info Management +800, Content Policy
  +800, Shorten Narrative Instructions +500, Emotion Images +500, Situation Images +500,
  Legacy Image Tagging no change.
- Documented the totals: enabling everything adds +5,500, taking Core Context from
  2,000 to 7,500 tokens.

## v2.0.2

- **Corrected `Is Start`.** The previous text said exactly one story node should be set
  to Yes. That was wrong — you can set it on several, and the reader then picks which
  opening situation to start from. The old wording discouraged a feature that works.

## v2.0.1

- Fixed the sidebar not tracking scroll position. Sections near the bottom of the page
  could never become active under the old method.

## v2.0

- First English release, rebuilt from the Korean guide.
- Added **Advanced Settings** and **Publish settings** sections.
- Added screenshots throughout.
- Established that Core Context is **2,000 tokens by default** — figures above that
  reflect Advanced Settings toggles, not a different baseline.
