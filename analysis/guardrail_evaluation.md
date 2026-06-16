# Task 8: Evaluate Guardrail Metrics

## Objective

Determine whether the Treatment group should be considered successful beyond conversion performance by evaluating operational, customer experience, and revenue quality guardrails.

---

## Primary Decision Principle

A treatment should not be adopted based only on higher conversion.

The experiment must also maintain healthy customer quality and operational outcomes.

---

## Guardrail Metric 1: Refund Rate

### Definition

Refund Rate = Refund Requests ÷ Total Users

### Why It Matters

Higher conversion can appear positive while creating low-quality purchases that later generate refunds.

### Evaluation Logic

* Lower or stable refund rate → acceptable outcome
* Higher refund rate → potential quality risk

### Risk Assessment

If Treatment shows a noticeable increase in refund requests, revenue quality may be lower and long-term value could decline.

Business implication:

* Avoid rollout if revenue growth is driven by unsustainable conversions.

---

## Guardrail Metric 2: Support Ticket Rate

### Definition

Support Ticket Rate = Users with Support Tickets ÷ Total Users

### Why It Matters

A treatment that increases customer confusion or onboarding friction creates operational cost.

### Evaluation Logic

* Stable or reduced support demand → healthy experience
* Increased support burden → implementation risk

### Risk Assessment

If support tickets rise after treatment exposure:

* onboarding may be unclear,
* product expectations may not match experience,
* support cost may offset conversion gains.

Business implication:

* Additional UX improvements may be required before rollout.

---

## Guardrail Metric 3: Average Days to Convert

### Definition

Average number of days required for converted users to become paying customers.

### Why It Matters

Fast conversion can indicate improved efficiency, but unusually fast conversion combined with refunds may indicate low purchase quality.

### Evaluation Logic

* Faster or stable conversion → positive signal
* Longer conversion cycle → friction risk

### Risk Assessment

If treatment causes longer conversion times:

* acquisition efficiency decreases,
* delayed revenue realization may impact business goals.

Business implication:

* Conversion speed should improve without reducing customer quality.

---

## Guardrail Metric 4: Average Engagement Score

### Definition

Average engagement score by experiment group.

### Why It Matters

Conversion without sustained engagement may indicate short-term gains rather than durable customer value.

### Evaluation Logic

* Stable or improved engagement → healthy adoption
* Lower engagement → retention concern

### Risk Assessment

If engagement declines:

* users may convert but fail to remain active.

Business implication:

* prioritize sustainable growth over temporary conversion lift.

---

## Additional Risk Check: Segment-Level Decline

Segments reviewed:

* Region
* Device Type
* Traffic Source
* Plan Type

### Evaluation Logic

Even if overall metrics improve, rollout should be reconsidered if specific segments experience decline.

Examples of risk:

* lower conversion in one region,
* increased refunds for one device type,
* lower engagement from specific traffic sources.

Business implication:

* consider partial rollout instead of full deployment.

---

## Final Guardrail Decision Framework

Proceed with treatment only if:

1. Primary conversion metric improves
2. Refund rate remains stable
3. Support ticket rate remains stable
4. Days to convert do not worsen materially
5. Engagement remains healthy
6. No critical segment-level decline appears

If one or more guardrails deteriorate meaningfully, the treatment should be revised before launch.
