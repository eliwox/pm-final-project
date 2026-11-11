# Feature Roadmap, Module 4 · BU Collection

**Scenario:** Riverty BU Collection, A Fair Way Forward

**Team:** [your assumed team size]

## Strategic anchors
- **Persona:** A consumer on shift or variable income, with one or more open claims, using the German portal, mostly on mobile. She wants a plan she can afford and keep, without making her situation worse.
- **Primary metric:** 60-day missed-payment rate for variable or shift agreements. Baseline is 22.5%, and the target is 20.5% or lower.
- **Moment of misery:** At the income question, Mara can’t tell whether “income” means this month or a normal month (N-01), why it’s asked, or how it’s used (T-206). She fears a wrong number could be used against her (N-06). She can’t see what a missed payment would cost, so she picks the plan that “looked like the right answer” and misses the second payment (N-02).
- **Guardrail:** Agreement rate for the segment, baseline 41.6% (46.0% overall), with no drop of more than 1 point. I’d also watch agent contact within 7 days, which should stay at or below 31.0%.

## Scoring
| Feature | Value | Effort | Quadrant | Decision | Rationale |
|---|---|---|---|---|---|
| B1 Income explainer | 4 | 1 | Quick Win | Now | It answers the moment of misery directly (N-01, T-206, N-06) and addresses the 16.2% of agent contacts asking why income is asked, but it clarifies rather than changes plan choice, so it is not a 5. |
| B2 Affordability check before plans | 5 | 3 | Major Project | Next | It is the only feature that acts where N-02 failed and where the 22.5% missed-payment rate is decided, so a rules-based version should fit the quarter, but it must be watched against the 41.6% agreement guardrail. |
| B3 One plan for several claims | 4 | 5 | Major Project | Next | The segment signal is strong (agreement 52.1% at one claim vs 27.6% at three or more), but it mainly lifts agreement, not the 22.5% metric, and it will not fit one quarter. |
| B4 Mobile upload fix or skip | 3 | 2 | Fill-In | Later | It protects the guardrail (853 journeys with a missing document, mobile agreement 43.8% vs 54.0%) but does nothing for missed payments. |
| B5 Pay-day payment date | 3 | 2 | Fill-In | Later | No interview or ticket mentions pay day, and variable earners may not have a fixed one, so its effect on the 22.5% is only a hypothesis. |
| B6 Agent handoff summary | 2 | 2 | Fill-In | Later | It fixes Daniel’s repeat questions (N-08, T-205), not Mara’s friction, and moves neither the primary metric nor the guardrail. |
| B7 Chat on every page | 2 | 3 | Time Sinker | Cut | Chat users miss more payments (21.6% vs 18.3%) and chat confirms plans without showing consequences (T-208), so scaling it risks the primary metric. |
| B8 Chat assistant on Shortest plan firstevery portal page | 1 | 1 | Fill-In | Later | Missed payments rose from 15.6% to 18.4% when Month 4 put the 6-month plan first, and N-02 shows people pick the first option, so this likely makes the primary metric worse. |

## Roadmap
### NOW, this sprint
- **B1 Income explainer**, It answers the moment of misery directly (N-01, T-206, N-06) and addresses the 16.2% of agent contacts asking why income is asked, but it clarifies rather than changes plan choice, so it is not a 5.

### NEXT, the following sprints
- **B2 Affordability check before plans**, It is the only feature that acts where N-02 failed and where the 22.5% missed-payment rate is decided, so a rules-based version should fit the quarter, but it must be watched against the 41.6% agreement guardrail.
- **B3 One plan for several claims**, The segment signal is strong (agreement 52.1% at one claim vs 27.6% at three or more), but it mainly lifts agreement, not the 22.5% metric, and it will not fit one quarter.

### LATER, backlog
- **B4 Mobile upload fix or skip**, It protects the guardrail (853 journeys with a missing document, mobile agreement 43.8% vs 54.0%) but does nothing for missed payments.
- **B5 Pay-day payment date**, No interview or ticket mentions pay day, and variable earners may not have a fixed one, so its effect on the 22.5% is only a hypothesis.
- **B6 Agent handoff summary**, It fixes Daniel’s repeat questions (N-08, T-205), not Mara’s friction, and moves neither the primary metric nor the guardrail.
- **B8 Chat assistant on Shortest plan firstevery portal page**, Missed payments rose from 15.6% to 18.4% when Month 4 put the 6-month plan first, and N-02 shows people pick the first option, so this likely makes the primary metric worse.

### ✂ Cut List
- **B7 Chat on every page**, Chat users miss more payments (21.6% vs 18.3%) and chat confirms plans without showing consequences (T-208), so scaling it risks the primary metric.
