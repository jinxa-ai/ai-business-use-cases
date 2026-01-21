# Use Case — AI-Assisted Lead Qualification

## Business Context
Organizations receive a high volume of inbound leads through multiple channels, with heterogeneous quality and intent.

## Problem Statement
Sales teams spend significant time manually reviewing and qualifying leads, leading to inefficiencies and missed opportunities.

## Why AI?
Natural language analysis enables early detection of intent, urgency and fit based on unstructured inputs.

## Proposed AI Approach (High-Level)
- Lead text classification
- Scoring based on intent and context
- Human validation loop before action

## Expected Benefits
- Faster lead response
- Improved sales focus
- Better prioritization

## Risks & Limitations
- Bias in training data
- Over-filtering valuable leads
- Lack of explainability if not designed carefully

## Cost & Governance Considerations
- Monitoring of inference costs
- Clear thresholds for automation
- Human override mechanisms

## When AI Is Not the Right Solution
Low lead volume or already structured qualification forms.

The effectiveness of this use case should be measured through a combination of speed, quality, and business impact indicators:

- **Time-to-First-Contact (TTFC)**  
  Reduction compared to baseline manual qualification.

- **Sales Acceptance Rate (SAR)**  
  Percentage of AI-qualified leads accepted by sales teams.

- **Conversion Rate Uplift**  
  Improvement from qualified lead to opportunity.

- **False Negative Rate**  
  Share of high-potential leads incorrectly deprioritized by AI.

- **Manual Override Rate**  
  Percentage of AI decisions modified by sales teams.

KPIs should be monitored weekly during initial rollout and monthly once stabilized.

## Risk Assessment

| Risk | Description | Level |
|------|-------------|-------|
| Misclassification | High-intent leads incorrectly scored as low value | 🟠 |
| Over-filtering | Excessive automation reducing pipeline volume | 🟠 |
| Bias amplification | Historical data reinforcing existing sales bias | 🟠 |
| Trust erosion | Sales teams losing confidence in AI recommendations | 🟠 |
| Cost drift | High inference volume on low-quality leads | 🟢 |

Mitigation principles:
- Conservative automation thresholds
- Mandatory human review for pipeline entry
- Regular bias and performance audits
- Transparent scoring explanations for sales teams

## Data Prerequisites Checklist

Before implementing this use case, the following conditions must be validated:

- [ ] Historical lead data available (minimum 6 months)
- [ ] Clear definition of “qualified lead” agreed with sales
- [ ] Access to unstructured lead content (messages, emails)
- [ ] Consistent CRM fields and pipeline stages
- [ ] Data ownership defined (sales / revops)
- [ ] Consent and compliance validated (PII, GDPR)
- [ ] Baseline metrics documented (current conversion, TTFC)

If multiple prerequisites are missing, AI qualification should be postponed in favor of process clarification.

## When AI Is Not the Right Solution

AI-assisted lead qualification is not appropriate when:
- lead volume is low and manageable manually
- qualification criteria are unclear or unstable
- sales teams lack trust in scoring mechanisms
- structured forms already capture sufficient qualification data

In these cases, improving form design and sales processes provides higher ROI than AI.

## Decision Summary

This use case is suitable for organizations with:
- medium to high lead volume
- heterogeneous lead sources
- established sales processes
- willingness to pilot AI as a decision support tool

AI should **augment sales judgment**, not replace it.

_This use case follows the principles defined in the AI-Consulting-Foundations repository._
