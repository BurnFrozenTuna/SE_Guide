# Changelog

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
