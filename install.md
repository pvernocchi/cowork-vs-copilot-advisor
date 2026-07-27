# 🛠️ Install `cowork-vs-copilot-advisor` in Cowork for M365 Copilot

This guide explains how to install the skill from this repository into **Cowork for M365 Copilot**.

---

## 1) Prerequisites

Before installation, ensure you have:

- Access to a Cowork workspace integrated with M365 Copilot
- Permission to create/import skills in that workspace
- This repository available locally or on GitHub:
  - `pvernocchi/cowork-vs-copilot-advisor`
- The skill file:
  - `SKILL.md`

---

## 2) Get the repository

Download the file `Skill.md` locally.

---

## 3) Review `SKILL.md`

Open `SKILL.md` and validate:

- Skill name and description match your intent
- Decision logic and guardrails are acceptable for your org
- Any org-specific wording is customized (if needed)

`SKILL.md` is the source of truth for behavior.

---

## 4) Import into Cowork

1. Open **Cowork for M365 Copilot**
2. Navigate to **Skills** (or **Skill Library**)
3. Select **Create Skill** / **Import Skill**

Then choose one method:

### Option A — Paste

- Copy all content from `SKILL.md`
- Paste into the skill editor
- Save

### Option B — Upload

- Use upload/import file
- Select `SKILL.md`
- Save

> UI labels can vary by environment/version.

---

## 5) Validate behavior

Run quick test prompts:

- “Should I use Cowork or M365 Copilot for summarizing this one doc?”
- “Should I run this multi-step transcript-to-deck workflow in Cowork?”

Expected behavior:

- Clear verdict
- 5-factor scorecard
- Cost-aware rationale
- [`precost`](https://github.com/Fepilot/cowork-precost-skill) recommendation when Cowork is advised

---

## 🧩 Troubleshooting

### Skill import fails

- Confirm file is named `SKILL.md`
- Ensure UTF-8 encoding
- Try paste mode if upload fails (or vice versa)

### Output seems inconsistent

- Check that the newest `SKILL.md` version is deployed
- Verify there are no conflicting instructions in the skill editor
- Add explicit examples to strengthen routing consistency

### Recommendation seems too generic

- Expand examples in `SKILL.md`
- Tighten decision boundaries for input/output complexity
- Add clearer assumptions and tie-breaker language
