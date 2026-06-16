# Task 7: Perform Hypothesis / A/B Test Analysis

## Objective

Evaluate whether the Treatment group generated a meaningful improvement compared with the Control group using the selected primary business metric.

---

## Summary of Test Inputs

### Primary Metric Tested

**Paid Conversion Rate**

Formula:

Paid Conversion Rate = Users Converted to Paid ÷ Total Users

### Groups Compared

* Control Group
* Treatment Group

### Test Type

Two-proportion hypothesis test (A/B test)

### Significance Level

[
\alpha = 0.05
]

---

## Hypotheses

### Null Hypothesis (H₀)

There is no statistically significant difference in paid conversion rate between Control and Treatment.

[
H_0 : p_{treatment}=p_{control}
]

---

### Alternative Hypothesis (H₁)

There is a statistically significant difference in paid conversion rate between Control and Treatment.

[
H_1 : p_{treatment}\neq p_{control}
]

---

## Test Output

The experiment compared paid conversion outcomes across both groups.

Record and insert:

* Control conversion rate
* Treatment conversion rate
* Test statistic (Z-score / equivalent)
* P-value

Example output structure:

| Measure                   | Result |
| ------------------------- | ------ |
| Control Conversion Rate   | XX%    |
| Treatment Conversion Rate | XX%    |
| Test Statistic            | X.XXXX |
| P-value                   | X.XXXX |

---

## Decision Rule

Decision threshold:

* If **P-value < 0.05** → Reject H₀
* If **P-value ≥ 0.05** → Fail to Reject H₀

---

## Business Interpretation

### Scenario 1 — Significant Result

If the p-value is below the threshold:

Interpretation:

* The treatment created a meaningful improvement in paid conversion performance.
* The business may consider rollout after validating guardrail metrics.

Business decision:

* Scale the treatment gradually.
* Continue monitoring refund rate, support burden, and engagement.

---

### Scenario 2 — Non-Significant Result

If the p-value exceeds the threshold:

Interpretation:

* Evidence is insufficient to conclude that the treatment improved conversion.

Business decision:

* Maintain the current experience.
* Design additional experiments or optimize the treatment before launch.

---

## Evidence File

Hypothesis test evidence saved as:

`screenshots/hypothesis_test_output.png`
