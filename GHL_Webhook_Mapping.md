# GHL Webhook Mapping Reference
## PatchitUP Franchise Application
## Webhook URL: https://services.leadconnectorhq.com/hooks/gN5lV0lMSTI7qdGs9YDJ/webhook-trigger/d626486f-1bdb-4973-a912-ab380d6edc14

---

## What to enter in GHL "Mapping" fields

In the GHL workflow trigger, you'll see two columns:
- **Left column** = the key name coming FROM the form (copy these exactly)
- **Right column** = the GHL field to map it TO (select from dropdown)

---

## Contact Fields (map to Contact object)

| Incoming Key | Maps To (GHL Field) |
|---|---|
| `first_name` | Contact → First Name |
| `last_name` | Contact → Last Name |
| `email` | Contact → Email |
| `phone` | Contact → Phone |
| `address` | Contact → Address |
| `city` | Contact → City |
| `state` | Contact → State |
| `postal_code` | Contact → Postal Code |

---

## Opportunity Fields (map to Opportunity object)

| Incoming Key | Maps To (GHL Field) |
|---|---|
| `territory_location_desired` | Opportunity → Territory Location Desired |
| `overall_fit_score` | Opportunity → Overall Fit Score |
| `job_title` | Opportunity → Job Title |
| `employer` | Opportunity → Employer |
| `education_level` | Opportunity → Education Level |
| `franchise_submission_date` | Opportunity → Franchise Submission Date |
| `liquid_capital` | Opportunity → Liquid Capital |
| `net_worth` | Opportunity → Net Worth |
| `credit_score` | Opportunity → Credit Score |
| `annual_income` | Opportunity → Annual Income |
| `needs_funding` | Opportunity → Needs Funding |
| `franchise_timeframe` | Opportunity → Franchise Timeframe |
| `who_runs_business` | Opportunity → Who Runs Business |
| `awareness_source` | Opportunity → Awareness Source |
| `frs_leadership_score` | Opportunity → FRS Leadership Score |
| `frs_sales_score` | Opportunity → FRS Sales Score |
| `frs_financial_score` | Opportunity → FRS Financial Score |
| `frs_technology_score` | Opportunity → FRS Technology Score |
| `frs_operations_score` | Opportunity → FRS Operations Score |
| `frs_culture_score` | Opportunity → FRS Culture Score |
| `frs_band_status` | Opportunity → FRS Band Status |
| `frs_band_tag` | Opportunity → FRS Band Tag |
| `ai_overall_verdict` | Opportunity → AI Overall Verdict |
| `ai_unit_recommendation` | Opportunity → AI Unit Recommendation |
| `ai_executive_summary` | Opportunity → AI Executive Summary |
| `ai_strength_1` | Opportunity → AI Strength 1 |
| `ai_strength_2` | Opportunity → AI Strength 2 |
| `ai_strength_3` | Opportunity → AI Strength 3 |
| `ai_strength_4` | Opportunity → AI Strength 4 |
| `ai_risk_1` | Opportunity → AI Risk 1 |
| `ai_risk_2` | Opportunity → AI Risk 2 |
| `ai_risk_3` | Opportunity → AI Risk 3 |
| `ai_training_area_1` | Opportunity → AI Training Area 1 |
| `ai_training_detail_1` | Opportunity → AI Training Detail 1 |
| `ai_training_area_2` | Opportunity → AI Training Area 2 |
| `ai_training_detail_2` | Opportunity → AI Training Detail 2 |
| `ai_training_area_3` | Opportunity → AI Training Area 3 |
| `ai_training_detail_3` | Opportunity → AI Training Detail 3 |
| `ai_next_step_1` | Opportunity → AI Next Step 1 |
| `ai_next_step_2` | Opportunity → AI Next Step 2 |
| `ai_next_step_3` | Opportunity → AI Next Step 3 |
| `why_patchitup` | Opportunity → Why PatchitUP |
| `franchise_goals` | Opportunity → Franchise Goals |
| `relevant_skills` | Opportunity → Relevant Skills |
| `job_responsibilities` | Opportunity → Job Responsibilities |

---

## Sample payload GHL will receive (for reference)

```json
{
  "first_name": "Marcus",
  "last_name": "Rivera",
  "email": "marcus.rivera@gmail.com",
  "phone": "(214) 555-0182",
  "address": "4821 Maple Ave",
  "city": "Dallas",
  "state": "TX",
  "postal_code": "75219",
  "territory_location_desired": "Dallas / Plano / Frisco, TX",
  "overall_fit_score": 3.42,
  "job_title": "Regional Operations Manager",
  "employer": "ServiceMaster Brands",
  "education_level": "Bachelor's Degree",
  "franchise_submission_date": "2026-03-23",
  "liquid_capital": "$100,000 – $149,999",
  "net_worth": "$250,000 – $499,999",
  "credit_score": "700 – 749 (Good)",
  "annual_income": "$100,000 – $149,999",
  "needs_funding": "Yes — SBA loan",
  "franchise_timeframe": "3 – 6 months",
  "who_runs_business": "I will — full-time owner-operator from day one",
  "awareness_source": "Google Search",
  "frs_leadership_score": 3.75,
  "frs_sales_score": 3.10,
  "frs_financial_score": 3.50,
  "frs_technology_score": 3.25,
  "frs_operations_score": 4.00,
  "frs_culture_score": 3.13,
  "frs_band_status": "Solid Candidate — Coaching Upside",
  "frs_band_tag": "FRS-Yellow",
  "ai_overall_verdict": "Promising Candidate",
  "ai_unit_recommendation": "Single-Unit Operator",
  "ai_executive_summary": "Marcus brings solid operational experience...",
  "ai_strength_1": "7+ years managing field teams in home services",
  "ai_strength_2": "Strong operations score (4.00)",
  "ai_strength_3": "Financially qualified with SBA path identified",
  "ai_strength_4": "Clear 3-year growth vision",
  "ai_risk_1": "Limited direct sales experience",
  "ai_risk_2": "Technology adoption will need support",
  "ai_risk_3": "Building culture from scratch is new territory",
  "ai_training_area_1": "Sales Execution",
  "ai_training_detail_1": "Focus on consultative close techniques",
  "ai_training_area_2": "CRM & Technology",
  "ai_training_detail_2": "Prioritize ServiceTitan hands-on training",
  "ai_training_area_3": "Culture Building",
  "ai_training_detail_3": "Walk through PatchitUP core values framework",
  "ai_next_step_1": "Schedule discovery call within 7 days",
  "ai_next_step_2": "Send territory availability report",
  "ai_next_step_3": "Connect with SBA lending partner",
  "why_patchitup": "I've spent years working inside a national home services brand...",
  "franchise_goals": "Year 1: Get to breakeven by month 6...",
  "relevant_skills": "I've managed teams of 8–14 field technicians...",
  "job_responsibilities": "Regional Operations Manager overseeing 3 markets..."
}
```

