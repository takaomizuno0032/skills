---
name: api-sequence-summary
version: 1.0.0
description: >
    Summarize Windows API call sequences from malware samples into
    abstract behavioral phases and attacker intent.
triggers:
    - malware analysis
    - マルウェア
    - API sequence
---

# API Sequence Summarization Skill

## Purpose

This skill converts **raw Windows API call sequences** into an
**abstract behavioral trace** that reflects attacker intent rather than
implementation details.

The goal is NOT to fully understand the code,
but to answer:

- What phases does this malware go through?
- What is it trying to achieve at each phase?
- What kind of malware lifecycle does this sequence imply?

Please provide a output in Japanese.

---

## Input Format

Provide a chronological list of Windows API calls.
Example:

```text
OpenProcess
VirtualAllocEx
WriteProcessMemory
CreateRemoteThread
Sleep
WinHttpSendRequest
```
