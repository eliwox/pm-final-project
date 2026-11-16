# GTM Launch Plan, Riverty BU Collection, A Fair Way Forward

| Field | Value |
|---|---|
| Feature | Inline income explainer on the income step of the instalment journey. |
| Goal | Conversion |
| Launch tier | S, Minimal |

## Goal & Audience
- **Goal:** Conversion, Consumers already reach the portal (8,360 starters a month), so awareness isn’t the gap. The feature exists to move a business metric: fewer plans that break within 60 days, which is 22.5% for variable or shift earners against 17.4% for fixed salary.
- **Target audience:** Primary: consumers on shift or variable income with one or more open claims who start an instalment journey in the German portal, mostly on mobile (2,862 starters a month, 34% of all starters; about 1,191 agreements). Secondary: collection agents in the pilot team, who field the “why is income asked?” contacts (16.2% of agent contacts).

## Launch Tier
- **S, Minimal**, The feature is copy inside an existing step, so the audience is already in the portal and needs no announcement. Reach is limited to about 2,862 starters a month, and revenue impact is unmeasured until the test reads out. The risk of silence is low for consumers. The real risk is agents who keep re-asking the same questions, so the only investment is internal enablement. A louder launch could also draw attention to data use, which N-06 shows already worries consumers.

## Channels
1. **Owned: The income step itself: the three plain statements shown beside the income field, where the misery happens. It reaches every variable or shift starter, 78% of them on mobile.**
2. **Owned: Collection agents: a briefing and one-pager so they point callers to the explainer instead of re-explaining. “Why income is asked” is 16.2% of agent contacts.**
3. **Owned: Client account managers: a short note for client reporting, since clients care about complaints and broken plans (N-10). I’m using no earned or paid channel, because paid promotion of collection outreach to financially stretched consumers would be inappropriate and unneeded.**

## Enablement & Assets
Compliance-approved German copy deck, including the retention period. Agent one-pager and FAQ on what the explainer says and how to refer to it. A client account manager note. A check that the chat assistant’s answers about income don’t contradict the explainer wording. Support briefed, no extra budget.

## Ownership, Budget & Timeline
- **Ownership & budget:** PM owns the plan and post-launch metrics. Compliance partner approves the copy and retention statement. UX writer owns German copy. Designer owns layout at 375 px. Front-end engineer owns the build and the randomization flag. Analyst owns the experiment read. Agent team lead owns the briefing. Client account manager owns the client note. No paid media budget. Extra cost: native German copy review and a copy test with about 8 variable-income consumers (amount to be confirmed). Asset gap: the approved retention period and the German copy deck.
- **Timeline:** Phase 1, beta: Weeks -2 to 0: compliance sign-off, segment assignment confirmed, agent one-pager drafted. Weeks 1 to 12: A/B enrolment (about 2.7 months), with weekly guardrail checks. Weeks 13 to 21: 60-day follow-up for the last people enrolled, and read at about week 21 (4.7 months). Phase 2, launch moment: Week 22: ship decision, roll out to 100% of the segment, agent briefing goes live, client note sent. Phase 3, post-launch: Weeks 23 and later: monitor the guardrail and diagnostics, with a review at about 90 days.

## Success Metrics
- **Metrics:** 60-day missed-payment rate, variable or shift agreements: 22.5% down to 18.5% or lower.
Share of agent contacts about “why income is asked”: 16.2% today. I’d set the target before launch; for example, 12% or lower is my proposal, not from the data.
Guardrail: agreement rate for the segment, baseline 41.6%, no more than 1 point below control (40.6%).
- **Bad signal to watch for:** Agreement rate falls to 40.6% or lower while missed payments improve. The explainer may be deterring people instead of helping them.
- **Likely post-launch decision:** Iterate. A copy-only change will probably land under the 4-point target (power is about 55% at 3 points and 28% at 2), so a significant 1 to 3.9 point improvement triggers pairing with the affordability check and a retest. Ship if the drop is 4 points or more, p < 0.05, and the guardrail holds.
