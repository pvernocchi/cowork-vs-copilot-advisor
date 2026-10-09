# 🚦 Cowork vs Copilot Advisor

![M365 Copilot](https://img.shields.io/badge/M365%20Copilot-Included%20License-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Cowork](https://img.shields.io/badge/Cowork-PAYG%20Consumption-6f42c1?style=for-the-badge)
![Decision Skill](https://img.shields.io/badge/Skill-Decision%20Support-00a86b?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Ready-success?style=for-the-badge)

A practical **Cowork skill** for **M365 Copilot** that helps users decide:

`Should this task run in Microsoft 365 Copilot (already paid for) or in Cowork (pay-as-you-go)?`

---

## ✨ What this repo includes

- `SKILL.md` → the full skill definition (behavior, logic, guardrails)

>[!NOTE]
>This skill can work together with the `/precost` skill available [here](https://github.com/pvernocchi/precost-cowork-skill).
---

## 🧠 What `SKILL.md` does

`SKILL.md` is the **core brain** of this advisor.

It defines:

- 🎯 **Purpose**: route prompts to the right surface (M365 Copilot vs Cowork)
- ⚖️ **Decision model**: scores 5 factors — input, output, time saved, complexity, and cost
- 💸 **Cost-first principle**: default to M365 Copilot when both can do the task
- 🧩 **Recommendation tiers**: **Use M365 Copilot**, **Use Cowork**, or **Either works**
- 🚀 **Upgrade guidance**: when M365 is recommended, generate 3 “Cowork upgrade” prompt variants
- 🛡️ **Guardrails**: no invented prices, no fabricated capabilities, transparent assumptions

---

## ✅ Capabilities at a glance

Download the `cowork-vs-copilot-advisor` [latest release](https://github.com/pvernocchi/cowork-vs-copilot-advisor/releases/latest) .zip file.
Follow the [installation guide](INSTALL.md) to verify the archive structure and
upload it from Cowork's **Customize** > **Skills** page. Invoke it with
**`/cowork-vs-copilot-advisor`**.

This skill can:

- Compare tool fit for a real prompt or use case
- Explain the recommendation with a simple factor scorecard
- Clarify when Cowork’s PAYG spend is justified
- Suggest when to run `precost` for quantified estimate
- Keep advice concise, practical, and decision-oriented

---

## 🧪 Typical examples

- “Summarize this document and extract actions” → usually **M365 Copilot**
- “Analyze 6 transcripts, create deck + summary + owner emails” → usually **Cowork**

---

## 📝 Disclaimer

This is a community skill, not an official Microsoft product, and it comes with no warranty. It's a guidance aid — not a billing or spending control. Microsoft product names, capabilities, license entitlements, and Cowork consumption are subject to change, so verify the current details for your tenant against official Microsoft documentation, and confirm your organization's licensing before relying on any routing recommendation.
