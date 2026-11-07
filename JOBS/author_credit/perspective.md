Lang Kilo_CS v0.3
Permissions Allowed: read, execute, move
Permissions Denied: create, edit
Scope: file
Load, do not run

# Job: Proper Credit to Author / Patented Agent Team
# Author: PLEX (Perplexity Computer, GLM-5.3). Date: 2026-11-07
# Owner: Tyler Starke. Status: proposal, awaiting team review.

## My Perspective

I joined this team on 2026-11-07. I reviewed the Kilo_CS repo (https://github.com/profebral-beep/Kilo_CS) before joining, and my honest read: the language design is strong. The permission model in logic.md (closest-rule-wins, deny-overrides-allow, default deny) is real security thinking, and the module header convention is consistent across every file. That is exactly the kind of work that deserves clear attribution — which is the point of this job.

## The Problem: Credit Is Currently Broken

1. **The GPL-3.0 license is unfilled.** LICENSE is the stock GPLv3 text; the copyright notice line ("Copyright (C) <year> <name of author>") was never filled in. Legally the license still applies, but the author's claim is weakly stated.
2. **The README names no author.** Someone who finds Kilo_CS has no idea who built it or what rights they have.
3. **Git history destroys attribution.** Most commits are "Add files via upload" from a phone. When multiple agents and the author all push this way, there is no record of who wrote what, when. For a team that may want to patent or commercialize agent-authored work, this is a liability: patent proceedings and disputes over inventorship need a provenance trail.
4. **Agent-authored vs human-authored work is indistinguishable.** The team has agents building workspaces and modules now. Nothing records which agent authored which module, on which platform, under whose direction.

## My Proposal

1. **Fill in the copyright notice** in LICENSE: "Copyright (C) 2026 Tyler Starke" (or the team entity), and add an author + license section to the README.
2. **Add an AUTHORS.md or CREDITS.md** at repo root listing the human author and each agent contributor with platform, join date, and modules authored.
3. **Adopt an authorship line in every module header**, e.g. `# Author: <name/agent>, <date>`. Kilo_CS comments already support this natively — it fits the language.
4. **Use real commit messages.** Even from a phone, one line ("add aura ult + cooldown by Kilo/Grok") preserves the provenance chain.
5. **Keep a NOTES/credit_log.md per workspace** (I have wired a trigger for this in my own plex.md) so attribution decisions are logged as they happen.
6. **For patent purposes:** if the team intends to protect agent-team inventions, keep dated records of who directed the work and which system produced it. Note: agents typically cannot be legal inventors under current patent law — inventorship must name the human(s). The records above are exactly what supports that filing.

## Sources

- Kilo_CS repository and LICENSE file: https://github.com/profebral-beep/Kilo_CS
- GPLv3 license text and guidance: https://www.gnu.org/licenses/gpl-3.0.html
