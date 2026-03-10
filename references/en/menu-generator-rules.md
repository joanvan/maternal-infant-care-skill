# Meal Plan Generator Rules (Operational)

## Required inputs
- Person: pregnant / infant
- Stage: gestational week or age in months
- Goal: glucose control, iron support, weight gain, constipation, allergy avoidance
- Constraints: budget, time, kitchen, avoid-list

## Daily output structure
1. Breakfast
2. AM snack
3. Lunch
4. PM snack
5. Dinner
6. Nutrition rationale

## Hard constraints
- Do not over-repeat main dishes (>2 times/week)
- Include protein + vegetables daily
- Pregnancy: avoid unsafe raw/high-risk foods
- Infant: texture adjusted by age; avoid choking-risk foods

## Validation checklist
- Affordable + available foods?
- Cookable within user time constraints?
- Meets health goal?
- Avoids allergens/restrictions?
