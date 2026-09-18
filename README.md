# Mathematical Paper Writing

A Codex skill for precise, restrained English mathematical research writing.

## Writing preferences

- Use concise prose to introduce a formula or derivation, followed by the explanation needed to understand it.
- Expand key estimates, uses of assumptions, and parameter choices; keep routine substitutions and repeated calculations concise.
- Introduce auxiliary notation when it has at least three substantive uses, with exceptions when notation clearly improves readability.
- Prefer distinct indexed constants for different estimates and state their relevant dependencies.
- In proofreading mode, edit English only. Preserve formulas, notation, proof order, paragraph structure, and citations; report mathematical or structural suggestions separately.
- Write manuscript text in English. Discussion and skill instructions may remain in Chinese.

The skill draws on writing patterns in selected papers by Kai Liu and collaborators, together with explicit writing preferences. Source observations and preferences are distinguished in the reference files.

## Install

Place this repository's contents in a directory named `mathematical-paper-writing` inside your Codex skills directory, normally `~/.codex/skills/`. The installed entry point should be `~/.codex/skills/mathematical-paper-writing/SKILL.md`.

## Use

```text
$mathematical-paper-writing Polish the English in this proof. Keep all formulas, notation, proof order, and paragraph structure unchanged.
```

```text
$mathematical-paper-writing Draft an English theorem and proof from these verified assumptions and derivations. State key estimates explicitly and keep routine calculations concise.
```

## Files

- [SKILL.md](SKILL.md): invocation scope, writing preferences, workflow, and editing boundaries.
- [style-profile.md](references/style-profile.md): detailed rules for prose, formulas, notation, proofs, and constants.
- [writing-patterns.md](references/writing-patterns.md): original examples illustrating the rules.
- [sources.md](references/sources.md): bibliographic sources and evidence locations.
- [openai.yaml](agents/openai.yaml): skill display metadata.

The source papers themselves are not included. The reference guide is self-contained for ordinary writing tasks.
