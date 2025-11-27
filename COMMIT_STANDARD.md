# CYW Commit Prefix Standard v1.0
Control Your World (CYW) — Repository Commit Convention  
Author: Timothy I. Wheels  
Version: v1.0  
Updated: CYW Timestamp Standard (UTC-05:00, EST)

This document defines the official commit prefix conventions for all CYW repositories, including:
- CYW OS frameworks
- VLAN routing logic
- Packets (A/B/C/D)
- Toolkits, templates, and onboarding systems
- Research and narrative assets

It blends industry-standard “Conventional Commits” with CYW-specific architectural layers.

---

## 🟦 Core Standard Prefixes (Universal)

| Prefix        | Purpose                                                        |
|---------------|----------------------------------------------------------------|
| **feat:**     | New feature, function, or capability                           |
| **fix:**      | Bug fix, patch, or broken logic correction                     |
| **docs:**     | Documentation only (README, comments, guides)                  |
| **style:**    | Formatting, typos, whitespace (no behavior change)             |
| **refactor:** | Structural improvement without altering behavior               |
| **perf:**     | Performance or optimization changes                            |
| **test:**     | Adding or updating tests                                       |
| **chore:**    | Maintenance tasks, renames, repo cleanup                       |
| **ci:**       | Continuous integration, workflows, GitHub Actions              |
| **build:**    | Build scripts, dependencies, environment tooling               |

---

## 🟩 CYW-Specific Prefixes (VLAN + Packet Architecture)

These map directly to the CYW OS design and your multi-layer workflow.

| Prefix        | Purpose                                                     |
|---------------|-------------------------------------------------------------|
| **cyw-core:** | Global CYW OS logic, systemic rules, protocols              |
| **vlan10:**   | Research updates, source gathering, external references     |
| **vlan20:**   | Synthesis, summarization, conversion to structure           |
| **vlan30:**   | Engineering, modules, scripts, technical build steps        |
| **vlan40:**   | Verification, QA, diagnostics, cross-checks                 |
| **vlan50:**   | Storytelling, branding, narrative, user-facing material     |
| **packet:**   | Packet creation, update, transformation (A/B/C builds)      |
| **os-spec:**  | Architecture specs, diagrams, routing logic, SOPs           |
| **notion:**   | Notion templates, JSON exports, dashboards                  |
| **slides:**   | Visual decks, slides, brand assets                          |

---

## 🟨 Optional Meta Prefixes

| Prefix       | Purpose                                           |
|--------------|---------------------------------------------------|
| **release:** | Version bumps (v1.0 → v1.1)                       |
| **hotfix:**  | High-urgency fix to broken production files       |
| **wip:**     | Work in progress (avoid on `main`)                |
| **meta:**    | Repo-wide configuration or non-code changes       |

---

## 🟥 Commit Message Format

Use the following structure:

```
<prefix>: short description

Optional extended description (what changed and why).
Refs: optional issue/packet/task link.
```

### Example
```
vlan20: integrate synthesis notes for Packet C-WhiteHouse

Added structure diagrams, updated research block, and clarified routing logic.
Refs: packet-C-WhiteHouse
```

---

## 🟪 Best Practices

- Keep the first line under **72 characters**.
- Use **present tense** (“add”, not “added”).
- Commit logically — do not bundle unrelated changes.
- Use CYW-specific prefixes for clarity and architecture alignment.
- Use `wip:` only on feature branches, not `main`.

---

### End of CYW Commit Prefix Standard v1.0
