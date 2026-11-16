# Experimentation Plan (Module 5)

## Get your documents ready
- **From M3, your hypothesis sentence:** Based on the interview evidence that variable-income consumers can’t tell which income the portal wants or what a missed payment costs (N-01, N-02), and the data showing they miss payments within 60 days at 22.5% versus 17.4% for fixed-salary consumers, I believe that explaining the income question and showing missed-payment consequences before plan selection for consumers on shift or variable income with open claims will result in more plans they can afford and keep, as measured by a 2-point reduction (22.5% to 20.5% or lower) in the 60-day missed-payment rate for this segment. I will protect the segment’s agreement rate (baseline 41.6%, no drop of more than 1 point) and will make a go/no-go decision after two full cohorts, about 3 months after launch.
- **From M3, your primary success metric & guardrail metric:** Primary: 60-day missed-payment rate, variable or shift agreements.
Guardrail: Agreement rate, variable or shift starters.
- **From M4, the feature you scoped in your PRD this is what you're testing:** Feature: The income explainer from the PRD. It adds three plain statements beside the income field: which income to enter, why it’s asked, and how the answer is used and kept.

## Define your experiment parameters
- **Feature under test pull from your M4 PRD:** Inline income explainer (three statements on the existing income step)
- **Persona pull your M2 persona:** Consumers on shift or variable income with open claims
- **Expected outcome the behaviour change you expect, from your M3 hypothesis:** Fewer plans that break within 60 days
- **Primary success metric the one number that defines success, from M3:** 60-day missed-payment rate (variable or shift agreements)
- **Baseline rate today's rate of your primary metric, from your M3 data:** 22.5%
- **Guardrail metric & boundary what must not break, and how far it can move before you investigate:** Agreement rate (baseline 41.6%); tripwire at 40.6% (1 point below control), checked weekly
- **Minimum Detectable Effect (MDE) the smallest improvement worth shipping, your floor:** 4 points (22.5% to 18.5%)
- **Sample size per arm use the calculator in the builder, baseline + MDE:** 1,598 agreements
- **Traffic split & test duration 50/50 standard · cover ≥ 2 weekly cycles:** 50/50, randomized by consumer, segment assigned before randomization. About 4.7 months (2.7 months of enrolment plus 60-day follow-up)
- **Significance threshold p < 0.05 is standard, explain any deviation:** p < 0.05, two-sided, 80% power

## Define your control and variant
- **Control (A) the current experience, reference your M2 moment of misery and M3 funnel/workflow data:** The current income step: no statement of which income is meant (N-01), why it’s asked or how it’s kept (T-206), or how data is used (N-06).
- **Variant (B) your single change, copy the relevant screens & functional requirements from your M4 PRD:** The same step plus three short statements beside the existing income field, each 25 words or fewer: which income to enter, why it’s asked, and how the answer is used and kept. Nothing else changes. Screens 1 and 3, the pay-pattern selector, the read-back, the new inline error area and the German number parsing are all removed from this test.
- **Isolation check, what has NOT changed? list everything identical between arms (app version, eligibility rules, notifications, onboarding). If something changed inadvertently, your test is compromised.:** App version and release; eligibility, outreach and entry channels; the income field and its validation; the affordability questions and income document step (including T-201); the plan screen, its ordering and all amounts; chat, agent screens and reminders (T-207); the segment definition; no other test running on the plan screen or chat.

## Formalize your hypothesis & shipping criteria
- **Your hypothesis (filled in):** believe that the inline income explainer will result in fewer plans that break within 60 days, as measured by a 4-point reduction (22.5% to 18.5%) in the 60-day missed-payment rate for variable or shift agreements, with a read at about 4.7 months. We will protect agreement rate (baseline 41.6%) throughout the test.
- **Your shipping criteria (filled in):** Ship	Missed-payment rate is 4.0 points or more lower (to 18.5% or better), p < 0.05, and agreement rate is no more than 1.0 point below control.
Hold and investigate	Agreement rate is 1.0 point or more below control at any weekly check, whatever the primary result.
Iterate	A significant improvement of 1.0 to 3.9 points. Pair the explainer with the affordability check and retest.
Inconclusive	Not significant and under 4 points. If a diagnostic hits its pre-set threshold, iterate; if none does, drop it.
Stop	Missed payments are 1.0 point or more higher in the variant, or agreement rate is clearly lower with no offsetting gain.
- **Hardest parameter to define, and did it change your hypothesis? quick debrief:** _(not filled in)_
