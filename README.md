# Human-Readable Diagnosis and Triage Skill

An Agent Skills-compatible workflow for explaining technical faults, confusing messages, screenshots, logs, and personal situations in plain Chinese.

## Style

The first answer should tell the user:

1. what probably happened;
2. how urgent it is;
3. what is actually confirmed;
4. what to do next safely.

Technical detail follows the decision, not the other way around.

## Evidence vocabulary

Use `CONFIRMED`, `SUPPORTED`, `POSSIBLE`, `UNKNOWN`, and `STALE` to make uncertainty visible.

## Safety

This skill provides triage and explanation, not medical, legal, financial, or psychological diagnosis. It also preserves logs and recovery options before risky system actions.

## Installation

Copy this directory into an Agent Skills-compatible skills directory, or install the repository with the client-specific skill manager.

## License

MIT. See [LICENSE](LICENSE).

