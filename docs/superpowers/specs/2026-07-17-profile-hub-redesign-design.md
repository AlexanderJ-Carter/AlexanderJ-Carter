# Profile Hub Redesign

Date: 2026-07-17

## Goal

Rewrite the GitHub profile hub so it reads as a warm personal identity with a clear research spine, and trim repository automation that does not serve a personal profile.

## Constraints (confirmed)

- Scope: README + repository hygiene together
- Tone: warm personal + academic/engineering blend
- Language: bilingual Chinese / English throughout
- Narrative: bold restructure around identity → research → projects → now/skills → snake → contact
- Authorship: cite AgentSociety 2 paper without emphasizing author order
- Automation: moderate trim (keep Profile CI, Snake, Link Check, Dependabot)

## Public facts used

- Name: Alexander / Haoyu Huang; Beijing; site alexander.xin; ORCID 0009-0007-0343-4129
- AgentSociety contributor (tsinghua-fib-lab/AgentSociety); co-author of AgentSociety 2 (arXiv:2607.11895)
- Related work: AgentSociety (arXiv:2502.08691) as platform background
- Own repos to feature: AgentSociety2-Agent-Skills, AlexanderJ-Carter.github.io, MIPS-Pipeline-Verilog, MyCook, netq / Git-Workflow-Lab as secondary

## README information architecture

1. Header + one-line positioning
2. About
3. Research (focus + collaboration)
4. Publications (standalone extensible table; ORCID canonical)
5. Projects (featured collaboration + selected pins)
6. Now + Skills (compact)
7. Snake (kept, lower)
8. Contact (deduped; points to publications + ORCID)

## Repository changes

- Remove unused `assets/signal-strip.svg`
- Remove release-drafter workflow and config
- Refresh `GOVERNANCE.md` and ignore patterns for new links
- Update featured SVG copy to match research positioning
- Keep Profile CI, Snake, Link Check, Dependabot, issue/PR templates

## Out of scope

- Inventing education/affiliation details not publicly stated
- Claiming authorship on AgentSociety v1 paper
- Pushing or merging without explicit user request
