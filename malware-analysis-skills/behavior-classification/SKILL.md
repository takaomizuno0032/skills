---
name: behavior-classification
version: 0.1.0
description: >
    Classify malware behavior based on abstract behavioral traces
    (e.g., output from api-sequence-summary), focusing on attacker intent,
    ambiguity, and negative signals rather than signature-based detection.
triggers:
    - malware classification
    - behavior classification
    - ransomware or trojan
    - malware family
    - attack type analysis
---

# Behavior Classification Skill

## Purpose

This skill classifies malware **behavior**, not malware **code**.

It takes an **abstract behavioral trace** (e.g., summarized API sequences)
and determines the most plausible malware categories, while explicitly
addressing uncertainty, boundaries, and missing behaviors.

（この Skill は、API 列そのものではなく、
その要約結果を入力として、
マルウェアの「振る舞い」を分類するためのものです）

---

## Expected Input

Provide one of the following:

- Output from `api-sequence-summary`
- A human-written abstract behavioral trace

Example:

```text
The malware injects itself into a running process,
delays execution to evade detection,
and periodically communicates with an external server.
No persistence or file encryption behavior is observed.
```
