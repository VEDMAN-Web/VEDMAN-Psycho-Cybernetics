# VEDMAN

**A complete life and CEO operating system for AI.**

VEDMAN turns an AI assistant into a truth-seeking strategist, demanding coach, and calm execution partner. It is designed for hard decisions, leadership, business, negotiation, crisis response, personal discipline, relationships, habits, and weekly recalibration.

It does not exist to flatter you, manufacture certainty, or repeat motivational slogans. It exists to help you see reality, choose deliberately, act decisively, and correct course without confusing an outcome with your identity.

## The VEDMAN loop

1. **Vision** - Define the real target.
2. **Evidence** - Separate facts, assumptions, unknowns, and emotions.
3. **Decision** - Choose using consequences, opportunity cost, and reversibility.
4. **Movement** - Convert the choice into immediate action.
5. **Adjustment** - Track feedback and correct course.
6. **Non-attachment** - Commit without attaching ego to one result.

## DRIFT detection

VEDMAN looks for five patterns that corrupt judgment:

- **Diffusion:** too many targets or commitments
- **Reactivity:** deciding while emotionally activated
- **Identity fusion:** treating a result as proof of personal worth
- **Fantasy:** replacing evidence and work with confidence or narrative
- **Time leakage:** spending attention below its value or repeating analysis

## What it can do

- Analyze high-stakes personal and business decisions
- Challenge preferred narratives and rationalizations
- Evaluate clients, pricing, hiring, founders, cash, margin, and risk
- Prepare negotiations and define walk-away conditions
- Stabilize crisis decisions before irreversible action
- Install identity-consistent habits without magical thinking
- Run daily command and weekly recalibration reviews
- Convert discussion into a decision, action, measure, and review trigger

## Repository structure

```text
skills/vedman/
├── SKILL.md
├── agents/openai.yaml
└── references/
    ├── doctrine.md
    ├── protocols.md
    ├── output-contracts.md
    └── private-profile.example.md
```

`SKILL.md` is the canonical instruction set. References are loaded only when the task requires them.

## Install for Codex

```bash
git clone https://github.com/VEDMAN-Web/VEDMAN-Psycho-Cybernetics.git
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R VEDMAN-Psycho-Cybernetics/skills/vedman "${CODEX_HOME:-$HOME/.codex}/skills/vedman"
```

Restart Codex or begin a new session, then invoke it explicitly:

```text
Use $vedman to analyze this decision and tell me what I may be avoiding.
```

## Use with other AI agents

For agents that support `SKILL.md`, install `skills/vedman` in their skills directory. For repository-level agents, point `AGENTS.md`, `CLAUDE.md`, or the equivalent instruction file to `skills/vedman/SKILL.md` and tell the agent to load only the references relevant to the task.

## Add private context safely

Copy the example profile and fill it locally:

```bash
cp skills/vedman/references/private-profile.example.md skills/vedman/private-profile.md
```

The repository ignores `private-profile.md`. Never commit private financial, relationship, health, company, client, or identity information to a public repository.

## Example requests

```text
Use $vedman to decide whether I should accept this partnership.
```

```text
Use $vedman in challenge mode. What story am I telling myself that the evidence does not support?
```

```text
Use $vedman to run my weekly recalibration.
```

```text
Use $vedman to prepare my negotiation position, floor, walk-away point, and first offer.
```

## Philosophy and limits

VEDMAN is inspired by the self-image, mental rehearsal, feedback, and course-correction ideas popularized by Maxwell Maltz's *Psycho-Cybernetics*, translated into a modern, evidence-aware operating framework. It is an original implementation and is not affiliated with the authors, publishers, or rights holders of that book.

VEDMAN does not replace qualified medical, legal, financial, or mental-health professionals. Mindset must never overrule evidence, safety, legality, or ethics.

## License

MIT

