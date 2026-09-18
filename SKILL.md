---
name: human-readable-diagnosis
description: Use when explaining crashes, errors, logs, screenshots, confusing system messages, or personal situations in plain Chinese. Lead with a human-language conclusion, urgency, evidence limits, and safe next steps without inventing certainty or making clinical diagnoses.
---

# Human-Readable Diagnosis and Triage

## Purpose

Translate confusing technical or personal situations into a short, honest, actionable explanation. Start with what the person needs to know now, then add technical detail only when it helps decide the next step.

“Diagnosis” here means evidence-based triage and explanation. It is not a medical, legal, financial, or psychological diagnosis.

## Activate when

- The user asks “这是什么”“说人话”“严重吗”“怎么办” about an error, crash, log, screenshot, warning, or system behavior.
- The user provides incomplete evidence and needs help separating facts from guesses.
- The user asks for plain-language interpretation of a personal conversation or confusing interaction.
- The answer could cause data loss, unsafe hardware action, medical delay, legal exposure, or financial loss.

## Core evidence levels

Use explicit levels:

- `CONFIRMED`: directly shown by a current log, file, measurement, or quoted message;
- `SUPPORTED`: consistent with the evidence but not uniquely established;
- `POSSIBLE`: a plausible hypothesis needing a discriminating check;
- `UNKNOWN`: the evidence does not support a conclusion;
- `STALE`: historical or reused evidence that needs refreshing.

Never convert a screenshot, one error code, a guessed PID, or a single message into a definitive root cause.

## Operating procedure

### 1. Start with the human-language conclusion

Answer in 1–3 short sentences:

- what most likely happened in ordinary language;
- whether it is urgent, dangerous, or safe to pause;
- what the user should avoid doing immediately.

Do not begin with a long acronym list or a wall of logs.

### 2. State the evidence boundary

Separate:

- what is directly observed;
- what is inferred from the observation;
- what cannot be determined yet;
- what evidence would distinguish the leading possibilities.

If the source is only a screenshot or partial quote, say so. Ask for the smallest useful missing artifact, such as a timestamped log, dump, exact command, file path, or full message context.

### 3. Rank causes by usefulness, not drama

Offer a short list of likely explanations. For each one, include the observation that supports it and the next check that could falsify it. Prefer common, reversible, and evidence-supported causes before rare catastrophic ones.

For technical faults, distinguish symptom, trigger, root cause, and impact. A stop code identifies a failure class; it does not by itself identify the offending driver or file.

For personal conversations, describe observable wording, timing, role, and context. Do not assign MBTI, attachment style, personality disorder, intent, or moral character as a fact from a fragment.

### 4. Give safe next steps

Order actions from least risky to more invasive:

1. preserve the current evidence;
2. run a read-only or reversible check;
3. back up before changing files, settings, or devices;
4. apply one focused change;
5. re-check and compare against the baseline.

When a situation is high-stakes, recommend the appropriate qualified professional or official support path. Do not encourage bypassing safety controls.

### 5. Close with a decision point

Tell the user what result would mean:

- if check A is true, follow path A;
- if check A is false, follow path B;
- if the check cannot be performed, report the limitation rather than guessing.

## Response contract

Use this compact structure:

1. `人话结论`
2. `紧急程度`
3. `已确认`
4. `最可能的解释`
5. `还不能确认`
6. `现在做什么`
7. `需要补充的证据`

Keep the first screen readable. Put codes, commands, and deeper theory after the plain-language explanation.

## Safety boundaries

- Do not claim a medical or mental-health diagnosis from chat text.
- Do not identify a legal violation, financial outcome, or malicious intent without adequate evidence.
- Do not recommend deleting dumps, clearing locks, resetting repositories, wiping devices, or changing protected system files before verifying the exact target and preserving recovery options.
- Do not treat the current date, an old memory, or a previous session as live evidence.

