# Humanizer (Westway Digital edition)

A Claude skill that rewrites AI-sounding text so it reads like the writer, without changing what it says.

This is an adapted copy of [blader/humanizer](https://github.com/blader/humanizer) v3.1.0 (upstream commit `8c307f3`, October 16, 2026). The patterns come from Wikipedia's [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing).

## Changes from upstream

- **Dashes are banned outright.** Upstream keeps em and en dashes when the writer's sample uses them. Here the rewrite never contains them, sample or not (§8 and the Voice section).
- **Section G, house patterns (§27 to §30):**
  - §27 Audience-widening and false ranges ("Whether you're X or Y", "From X to Y")
  - §28 Business buzzwords (leverage, seamless, streamline, empower, synergy, best-in-class, and others)
  - §29 Filler, stock openers, and announced endings ("in order to", "it's worth noting", "In today's fast-paced world", "In conclusion")
  - §30 Stiff transitions and hollow intensifiers (Moreover, Furthermore, very, truly, incredibly)

Everything else matches upstream.

## Install

- **Claude (web or desktop):** download this repo as a ZIP and upload it as a skill in Settings.
- **Claude Code and other agents:** `npx skills add westwaydigital/humanizer`

## Pulling in upstream changes

This copy does not update itself. When upstream releases a new version, merge its `SKILL.md` changes by hand and keep the dash rule and section G.

## License

MIT. Original work Copyright (c) 2025 Siqi Chen. See [LICENSE](LICENSE).
