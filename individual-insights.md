# Individual Insights

## My story

I worked on the Riverty BU Collection case, where consumers abandon digital repayment plans. The data showed the biggest drop at the income step (only 77.9% continue to plan review), and 16.2% of agent contacts were about why income is asked. That pointed to one specific moment of misery: Mara, a shift worker with several claims, reaches the income form, doesn't know whether "income" means this month or a normal month, and leaves.

From there I scoped a single feature, a plain explainer for why income is asked, and planned how to test and launch it: an A/B test aiming for agreement rate 46% → 50% while protecting the 60-day missed-payment rate, then an S-tier launch with no outreach and owned channels only.

## Key takeaways

1. **The guardrail matters as much as the goal.** Showing the shortest plan first raised agreement but also raised missed payments (15.6% → 19.0%). That is why the missed-payment rate became a guardrail with a clear boundary instead of an afterthought.
2. **Prototyping exposed a gap in my PRD.** Trust information only lived inside the explainer. Building the prototype showed users need reassurance before they open it, so I moved a short reassurance onto the income-entry screen.
3. **Sample size changed my plan.** In Module 3 I planned to decide after 1,000 journeys. Detecting a +4 pp lift from a 46% baseline needs roughly 2,450 per arm, so the test window had to be longer.
4. **AI executes, the PM decides.** The AI summary smoothed over the specific income-form frustration into generic bullets, and the strategy only became useful once I brought the JTBD, effort/impact and retention thinking myself.
5. **Match the launch to the feature.** The feature lives inside an existing flow, so conversion and a small, internal-facing launch fit better than awareness.

## What I would do next

- Run the A/B test and read the result only at the fixed read date.
- Confirm the data retention period with legal before the explainer states anything about it.
- If the shipping criteria are met, move on to B3, the affordability check before plan options.
