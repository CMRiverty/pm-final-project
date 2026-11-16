# A/B Experiment Brief, Riverty BU Collection, A Fair Way Forward

## Parameters
| Parameter | Decision |
|---|---|
| Feature under test | B2 – Plain income explainer on the income-entry screen |
| Persona | Mara the Hesitant Planner: a shift worker with multiple open claims and variable income who wants to set up a repayment plan digitally. |
| Expected outcome | Expected outcome: More hesitant planners continue past the income step and agree to a repayment plan online, without contacting an agent. |
| Primary success metric | Primary success metric: Repayment-plan agreement rate. |
| Baseline rate | Baseline rate: 46.0% |
| Guardrail metric | 60-day missed-payment rate (baseline 19.0%) |
| Guardrail boundary | Must not reach 20.0% (+1 percentage point); investigate if it does. |
| Second guardrail | · |
| Minimum Detectable Effect | +4 pts |
| Sample size per arm | 2 448 |
| Traffic split | · |
| Test duration | Minimum 14 days (≥ 2 weekly cycles), or until the sample size per arm is reached |
| Significance threshold | p < 0.05 (95%) |

## Control vs. Variant
- **Control (A):** The current income-entry screen, which asks for income without explaining why it is needed or how it is used. Only 77.9% continue from the income document step to plan review, and users abandon because they don’t know whether “income” means this month or a normal month (N-01).
- **Variant (B):** The same income-entry screen with one change: a short reassurance text at the top of the screen, and a full explanation one tap away covering why income is asked, how it affects plan recommendations, how data is stored and protected, and why accurate income helps the customer.
- **Held constant (isolation check):** App version, eligibility rules, income questions and fields, document upload flow, plan options and their order, reminders and notifications, onboarding, and agent screens are identical in both arms

## Hypothesis
> I believe that B2 – Plain income explainer on the income-entry screen for Mara the Hesitant Planner: a shift worker with multiple open claims and variable income who wants to set up a repayment plan digitally. will result in Expected outcome: More hesitant planners continue past the income step and agree to a repayment plan online, without contacting an agent., as measured by a +4 pts change in Primary success metric: Repayment-plan agreement rate. within Minimum 14 days (≥ 2 weekly cycles), or until the sample size per arm is reached. We will protect 60-day missed-payment rate (baseline 19.0%) throughout the test.

## Shipping criteria
> We will **ship** if Primary success metric: Repayment-plan agreement rate. improves by ≥ +4 pts at p < 0.05 (95%) and 60-day missed-payment rate (baseline 19.0%) does not reach Must not reach 20.0% (+1 percentage point); investigate if it does. after Minimum 14 days (≥ 2 weekly cycles), or until the sample size per arm is reached.
> We will **iterate** if direction is positive but lift is below the MDE.
> We will **kill** if the primary metric shows no improvement or moves negatively.
> The read date is fixed at the end of Minimum 14 days (≥ 2 weekly cycles), or until the sample size per arm is reached, no results reviewed before this date.
