# AI Synthesis, Product Health & Insights Summary (Module 2)

## Responses
- **Assumption to validate #1:** Consumers abandon the instalment-plan journey primarily because of confusion and lack of trust, not because they are unwilling or unable to pay.
- **Assumption to validate #2:** Providing clearer explanations and recommendations will increase self-service plan creation without increasing failed repayment plans.
- **Assumption to validate #3:** A significant share of agent contacts related to instalment plans can be prevented through a better digital journey and clearer guidance.
- **Moment of misery / red flag #1 (e.g., “user gave up after 3 tries”):** Confusion During Affordability Assessment
- **Moment of misery / red flag #2:** Lack of Trust Before Commitment
- **Moment of misery / red flag #3:** Agreeing Without Understanding the Consequences
- **Product Health & Insights Summary (Claude's output):** # Product Health & Insights Summary

## Executive Summary

The platform is technically functional but fails users at the moments that matter most: entering financial information, committing to a plan, and understanding the consequences. Stability defects (upload timeouts, data loss on navigation, late reminders) and data inconsistencies (portal amounts that differ from letters) are eroding user confidence and driving consumers back to phone channels. The result is a self-service experience that generates rework for agents, risk for clients and compliance, and hardship for consumers who may already be in a fragile financial position.

## Thematic Synthesis

### 1. Technical Stability & Data Integrity

Several defects interrupt completion of the digital journey or produce incorrect outputs. The most significant is the failure of document upload on mobile, which affects a very large share of journeys. Data-consistency issues between the portal and outbound letters compound this, particularly in purchased portfolio cases, where underlying data quality is also uneven.

- **Income document upload times out on mobile for large photos** (T-201). 853 journeys in the sample month requested a document that never arrived. Severity: **Critical**
- **Portal amount differs from the letter** (T-203). 531 journeys in the sample month, 343 of them purchased portfolio cases. Severity: **Critical**
- **Reminder before the first instalment sometimes arrives after the due date** (T-207). Directly contributes to missed payments. Severity: **High**
- **Back button on the plan review screen clears affordability answers** (T-204). Forces users to re-enter sensitive data and risks abandonment. Severity: **High**
- **Inconsistent data across acquired portfolios** (N-11). Some lack reliable phone or address history, limiting both digital and agent-led contact. Severity: **Medium**

### 2. Onboarding & Journey Design

The journey assumes a single-claim, single-plan, stable-income consumer. Users with multiple claims or irregular income (such as shift workers) cannot map their circumstances onto the flow. Ambiguous questions and a plan selection that nudges users toward a shorter term produced real affordability failures.

- **No way to set up one plan across multiple claims; claims are shown individually** (T-202, N-03). Users cannot tell whether paying one claim stops contact about another. Severity: **High**
- **Ambiguous income question** (N-01). It is unclear whether "income" means this month or a typical month, leading to abandonment mid-journey. Severity: **High**
- **Plan options that mislead on affordability** (N-02). The lowest-month plan appears to be the "right" answer, but its higher amount led to a missed second payment. Severity: **High**
- **Preference for phone over digital** (N-04). Some users want human reassurance on cost, signalling gaps in the digital channel's explanatory power. Severity: **Medium**

### 3. Trust, Clarity & Transparency

Consumers are asked for sensitive financial data without being told why it is needed, how it will be used, or how long it is retained. The chat assistant compounds the problem by confirming plans quickly without explaining the downside of missing a payment. Fear of data misuse is most acute among users who are already financially stretched.

- **No explanation of why income is requested or how long it is kept** (T-206, N-06). Users fear their input will be used against them. Severity: **High**
- **Chat assistant confirms plans without showing missed-payment consequences** (T-208, N-05). Speed is valued, but users commit without understanding the risk. Severity: **High**
- **Amount mismatches cause users to withhold agreement** (N-07). Users defer commitment until a person explains the discrepancy. Severity: **High**

### 4. Agent Enablement & Support Load

Agents have no visibility into what consumers entered online or why a plan was offered. This forces duplicated data collection on calls and leaves agents unable to diagnose failed plans. The digital channel is therefore generating additional work rather than deflecting it.

- **Agent screen shows neither consumer inputs nor the rationale for an offered plan** (T-205, N-08, N-09). Roughly half of calls begin with re-collection of details already provided. Severity: **High**
- **Failed plans cannot be explained after the fact** (N-09). Agents see only a number, limiting their ability to remediate. Severity: **Medium**

### 5. Client, Commercial & Compliance Exposure

Client-side stakeholders weigh complaints alongside recovery performance, and broken plans are visible in client reporting. Compliance requires that decisions be explainable to both consumers and agents, a standard the current experience does not meet given the opacity in plan offers and amount discrepancies.

- **Broken plans surface in client complaint and performance reporting** (N-10). Severity: **High**
- **Decision logic is not explainable to consumers or agents** (N-12). Creates regulatory and conduct risk. Severity: **High**

### Minor Technical Debt

Isolated, low-impact items not tied to the recurring themes above, including minor copy and labelling inconsistencies, edge-case display issues, and non-critical data gaps in acquired portfolio records. Severity: **Low**
- **Did the AI catch the specific moment of misery / pain point you found in Step 1?:** Partly
- **Did it smooth over a critical frustration into a generic bullet point?:** Yes
- **Did the AI try to suggest features or a roadmap despite the constraints?:** No
- **Logic leak / hallucination #1 (e.g., “AI suggested a new search bar feature, roadmap leak”):** _(not filled in)_
- **Logic leak / hallucination #2:** _(not filled in)_
