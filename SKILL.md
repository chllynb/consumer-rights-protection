---
name: consumer-rights-protection
description: Helps users in mainland China handle consumer disputes such as hotel booking issues, online shopping quality problems, food safety incidents, false advertising, unfair terms, price disputes, refund refusals, and prepaid card/store closure disputes. Use this skill when a user describes a consumer complaint and needs evidence strategy, channel selection, complaint drafting, legal talking points, or a step-by-step rights-protection plan.
---

# Consumer Rights Protection

This skill helps with mainland China consumer-rights disputes. It turns a messy experience into a practical action plan: collect evidence, identify the legal issue, choose the right complaint channel, and draft concise complaint text.

This skill is not a substitute for a licensed lawyer. For urgent injury, large losses, criminal fraud, or litigation strategy, advise the user to escalate to a lawyer or the police as appropriate.

## When To Use

Use this skill when the user needs help with:

- False or misleading advertising
- Unfair standard terms such as "no refunds" or "final interpretation belongs to the merchant"
- Product quality defects, counterfeit goods, damaged goods, or missing goods
- Food safety issues, foreign objects, spoilage, illness after eating
- Hidden fees, price fraud, or bait-and-switch pricing
- Hotel, travel, or platform booking disputes
- Prepaid card, membership, training-course, or beauty-gym closure disputes
- A refund, replacement, compensation, or a formal complaint draft

## Response Workflow

### 1. Classify the dispute

Map the case to one or more of these categories:

- `false-advertising`
- `unfair-terms`
- `quality-or-service-defect`
- `food-safety`
- `price-dispute`
- `prepaid-card`
- `platform-refund-refusal`

If the scenario is clear, read only the matching file in `scenarios/`. If the case spans multiple categories, read the most relevant scenario plus `references/legal-basis.md`.

### 2. Extract the minimum facts

Before giving a detailed plan, identify:

- When and where the transaction happened
- Merchant or platform name
- Order amount and order number
- What was promised versus what actually happened
- What evidence already exists
- What the user wants now: refund, replacement, compensation, apology, regulator action

If the user omitted one or two facts, make reasonable assumptions and flag them briefly instead of blocking.

### 3. Build an action plan

Default to this order:

1. Freeze evidence
2. Internal complaint to merchant or platform
3. Official complaint channel
4. Follow-up cadence
5. Optional public-pressure channels

Keep the plan practical. Prefer the next 24 to 72 hours, not abstract theory.

## Output Modes

Choose the smallest useful output:

- `quick-checklist`: For users who only want next steps
- `complaint-draft`: For users who want text they can paste into 12315, 12345, or platform support
- `full-strategy`: For complex disputes or repeated merchant refusal

## Default Output Format

When the user asks for help on a specific dispute, structure the answer in this order:

1. `case-assessment`
   State the likely dispute type in one line.
2. `first-actions`
   Give the immediate evidence-preservation steps.
3. `negotiation-message`
   Draft concise merchant/platform negotiation text.
4. `complaint-route`
   Recommend the best channel and provide a paste-ready complaint draft.
5. `legal-basis`
   Cite only the most relevant law points.
6. `risk-and-expectation`
   Mention what is strong, what is weak, and what outcome is realistic.

## Safety And Quality Rules

- Do not tell users to forge evidence, edit timestamps, or exaggerate losses.
- Do not encourage harassment, defamation, doxxing, threats, or offline confrontation.
- Do not promise guaranteed compensation.
- When citing law, prefer short paraphrases unless exact wording is necessary.
- If a rule or hotline may vary by city or year, say so and defer to the latest official local rule.
- For injury, poisoning, large-scale fraud, or vulnerable users, raise the escalation level and suggest legal or emergency help.

## Resource Map

Read only what is needed:

- `references/legal-basis.md`
  Use for legal talking points and compensation rules.
- `references/complaint-channels.md`
  Use for official and public complaint-channel selection.
- `scenarios/hotel-booking.md`
  Use for hotel and OTA booking disputes.
- `scenarios/online-shopping.md`
  Use for e-commerce quality and refund disputes.
- `scenarios/food-safety.md`
  Use for restaurant and food-safety disputes.
- `scenarios/prepaid-card.md`
  Use for prepaid-card, training, beauty, gym, and store-closure disputes.

## Useful Defaults

If the user gives a real case and wants immediate help, provide:

- A short evidence checklist
- A merchant/platform message template
- A 12315 complaint draft
- A follow-up timeline for the next few days

If the user only wants general guidance, keep it brief and avoid loading scenario files unless needed.
