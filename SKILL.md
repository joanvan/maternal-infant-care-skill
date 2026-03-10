---
name: maternal-infant-care
description: Bilingual maternal-infant lifecycle support skill (Chinese/English): preconception, pregnancy, postpartum, newborn and infant (0-3 years), with practical triage, 30-day planning, nutrition/menu generation, and caregiver execution checklists. Use when users ask for maternal/infant daily care plans, symptom triage, feeding/sleep routines, growth/development support, or doctor-visit preparation.
---

# Maternal Infant Care

## Safety first

1. Triage before advice (urgent vs same-day vs home observation).
2. This skill does not replace diagnosis or emergency care.
3. If data is missing, ask for week/month age, vitals, feeding/urine, mental status first.
4. Output must be actionable: **what to do now, when to recheck, when to seek care**.

## Language routing

- Chinese user -> prioritize `references/zh/`
- English user -> prioritize `references/en/`
- If an English topic is missing, adapt from Chinese source with clear wording.

## Workflow

### Step 1: Identify subject and stage
- Mother: preconception / trimester / postpartum
- Child: newborn (0-28d) / infant (1-12m) / toddler (1-3y)

### Step 2: Risk stratification
- Use `references/zh/red-flags.md` (or equivalent English triage logic)
- Return red/yellow/green decision with next action.

### Step 3: Choose topic module

Core operational modules:
- Pregnancy: `references/zh/pregnancy.md` | `references/en/pregnancy.md`
- Newborn fever pathway: `references/zh/newborn-fever-pathway.md` | `references/en/newborn-fever-pathway.md`
- 30-day plans: `references/zh/monthly-plans-template.md` | `references/en/monthly-plans-template.md`
- Menu generator: `references/zh/menu-generator-rules.md` | `references/en/menu-generator-rules.md`
- GDM plan: `references/zh/gestational-diabetes-meal-plan.md` | `references/en/gestational-diabetes-meal-plan.md`

Extended Chinese library (full set):
- `references/zh/*.md`

### Step 4: Response format
1) Current assessment (stage + risk level)
2) Immediate 3-5 actions
3) Observation metrics (temperature/urine/feeding/alertness etc.)
4) Recheck timing
5) Escalation triggers
6) Copy-paste doctor summary
