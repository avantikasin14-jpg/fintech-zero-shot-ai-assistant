# fintech-zero-shot-ai-assistant
An evidence-based FinTech prompt engineering portfolio demonstrating zero-shot AI workflows for EMI verification, complaint triage, factual summarization, and customer communications, with independent evaluation and responsible AI controls.
# FinTech Zero-Shot AI Assistant

### Applied Generative AI | Prompt Engineering | FinTech

**Institution:** Chitkara University  
**Program:** BBA FinTech  
**Lab:** 1 — Zero-Shot Prompting  
**Student:** [Avantika] 
**Student ID:** [2620992550] 
**Academic Session:** 2026–2027  
**AI Tool/Model:** [ChatGPT - GPT-6]
**Status:** Educational Prototype

---

## 1. Executive Summary

This project demonstrates the application of zero-shot prompt engineering to four realistic FinTech business workflows:

1. EMI explanation and financial calculation verification.
2. Customer complaint classification and triage.
3. Evidence-based financial data summarization.
4. Multilingual customer communication and professional email drafting.

The project uses no-code Generative AI tools, manual verification, and documented evaluation procedures.

**Project Goal:** Explore how structured prompts can improve the clarity, reliability, and usefulness of AI-generated outputs in financial services.

## 2. Business Problem

FinTech organizations handle large volumes of customer questions, payment complaints, financial information, and operational communications.

Generative AI may assist employees with these activities, but incorrect calculations, misleading statements, and unsupported assumptions create business risks.

This project investigates whether carefully designed zero-shot prompts can support these workflows while maintaining human oversight.

## 3. Project Objectives

- Develop precise zero-shot prompts.
- Apply prompt engineering to financial services.
- Verify AI-generated financial calculations.
- Classify fictional customer complaints.
- Identify hallucinations and unsupported conclusions.
- Evaluate multilingual communication accuracy.
- Document reproducible experiments.
- Follow responsible AI principles.

## 4. Methodology

For each experiment:

1. Identify the business problem.
2. Create an initial zero-shot prompt.
3. Execute the prompt using an AI tool.
4. Record the original AI response.
5. Independently evaluate the response.
6. Improve the prompt.
7. Execute the revised prompt.
8. Compare the results.
9. Document observations and limitations.

No worked examples are supplied inside the zero-shot prompts.

## 5. Lab Experiments

### Task 1: EMI Explanation and Verification

**Business Application:** Customer financial education and loan information.

**Baseline Prompt:**

> Explain EMI to a first-year BBA FinTech student in 50 words.

**Improved Prompt:**

[Calculate the Equated Monthly Instalment (EMI) for a personal loan of ₹2,50,000 at an annual interest rate of 14% for a repayment period of 24 months.

Include:
1. The EMI formula.
2. Step-by-step substitution of the given values.
3. The calculated monthly EMI.
4. Total repayment over 24 months.
5. Total interest payable.

Present the final results in a clear table. Round all monetary values to two decimal places and explain the calculations in simple language suitable for a first-year BBA Fintech & AI student.]

The improved prompt should request:

- EMI formula
- Monthly EMI
- Total repayment
- Total interest
- Tabular output

**Independent Verification**

EMI formula:

EMI = P × r × (1 + r)^n / [(1 + r)^n − 1]

Where:

- P = ₹2,50,000
- r = 0.14 / 12
- n = 24 months

Spreadsheet formula:

`=250000*(14%/12)*(1+14%/12)^24/((1+14%/12)^24-1)`

**Record Results:**

| Metric | AI Result | Spreadsheet Result | Difference |
|---|---|---|---|
| Monthly EMI | [₹12,002.46] | [₹12,002.46] | [0.00] |
| Total Repayment | [₹2,88,059.04] | [₹2,88,059.04] | [0.00] |
| Total Interest | [₹38,059.04] | [₹38,059.04] | [0.00] |

**Conclusion:** [The AI calculations match the spreadsheet results, with no difference after rounding to two decimal places. This indicates that the EMI calculation is mathematically accurate for the given loan amount, interest rate, and tenure.]

### Task 2: Customer Complaint Classification

**Business Application:** Customer support ticket categorization.

**Objective:** Classify eight fictional customer complaints into:

- Payments
- Loans
- KYC/Account
- Needs review

**Prompt:**

[Act as a FinTech customer complaint classification assistant.
Classify each of the following 8 fictional customer complaints into exactly one category:
Payments: UPI, transfers, failed payments, refunds, or transaction issues.
Loans: EMI, loan repayment, interest, or loan-related deductions.
KYC/Account: Identity verification, account access, or account updates.
Needs review: Insufficient information to determine the correct category.
Customer Complaints:
UPI payment failed, but the amount was debited.
My EMI was deducted twice this month.
My PAN verification is still pending.
I transferred ₹5,000, but the recipient hasn't received it.
My loan interest rate increased unexpectedly.
My account is blocked after updating my KYC.
Money has disappeared from my account.
My application was rejected without explanation.
Instructions:
Assign exactly one category per complaint.
Do not invent missing information.
Mark ambiguous complaints as Needs review.
Provide a short reason for each classification.
Suggest one recommended action.
Return a table with four columns: Complaint, Category, Reason, and Recommended Action.
Do not provide classification examples before processing the complaints.
Then check every label yourself, list the ones you disagree with, and explain why]

**Expected Output Format:**

| Complaint | Category | Reason | Recommended Action |
|---|---|---|---|
| [Complaint] | [Category] | [Reason] | [Action] |

**Evaluation Questions:**

1. Did the model follow the classification rules?
2. Were ambiguous complaints marked Needs review?
3. Did the model invent missing information?
4. Were recommended actions appropriate?

**Manual Review:**

[**Incorrect or Disputed Classifications:** None.
**Review Findings:**
All eight classifications were consistent with the provided category definitions.
**Observation:** Complaint 2 (duplicate EMI deduction) could potentially be considered a Payments issue because it involves a duplicate debit. However, since the complaint specifically mentions EMI repayment, Loans is the more appropriate category.
**Final Assessment:** The model demonstrated consistent classification, appropriate ambiguity handling, and relevant recommendations]

### Task 3: Evidence-Based Summarization

**Business Application:** Financial operations reporting.

**Fictional Company:** PaySetu

**Source Information:**

- September transactions: 4.2 lakh
- October transactions: 5.1 lakh
- September average transaction value: ₹640
- October average transaction value: ₹590
- Server downtime increased in October
- Revenue and cost data are unavailable

**Task:**

Generate a three-bullet factual summary and identify conclusions that cannot be supported by the source information.

**Independent Calculations:**

September transaction value:

420,000 × ₹640 = ₹26.88 crore

October transaction value:

510,000 × ₹590 = ₹30.09 crore

**Evaluation:**

| Check | Observation |
|---|---|
| Accurate transaction figures | [Yes. September: 4.2 lakh; October: 5.1 lakh.] |
| Accurate calculations | [Yes. September: ₹26.88 crore; October: ₹30.09 crore.] |
| Unsupported revenue claims | [No revenue claims were made because revenue data was unavailable.] |
| Unsupported profitability claims | [No profitability conclusions were made because cost and revenue data were unavailable.] |
| Correct identification of missing data | [Yes. Revenue and cost information were correctly identified as unavailable.] |

**Conclusion:** [The AI-generated summary accurately represented the provided information and calculations. Transaction volume increased from 4.2 lakh in September to 5.1 lakh in October, while average transaction value decreased from ₹640 to ₹590. The estimated total transaction value increased from ₹26.88 crore to ₹30.09 crore.
The model correctly identified increased server downtime as an operational concern. It did not make unsupported claims about revenue or profitability.
Overall, the output demonstrated factual accuracy, appropriate calculations, and responsible handling of missing information]

### Task 4: Translation and Business Communication

**Business Application:** Customer communication and settlement operations.

**Part A: Translation**

Translate the provided failed-payment notification into Hindi.

Requirements:

- Preserve the original meaning.
- Do not invent refund timelines.
- Do not add unsupported commitments.
- Back-translate into English.
- Compare the original and translated versions.

**Part B: Professional Email**

Draft a 100-word email from an operations executive to a partner bank about a delayed settlement.

Use placeholders for:

- Transaction IDs
- Amounts
- Dates
- Account references

**Evaluation:**

| Criterion | Observation |
|---|---|
| Translation accuracy | [Not applicable to this task; it involves email drafting, not translation.] |
| Meaning preserved | [Yes. The email clearly communicates the delayed settlement issue and requests an update.] |
| Professional tone | [Yes. The language is formal, polite, and suitable for bank communication.] |
| Word-count compliance | [Yes. The email body was approximately 100 words.] |
| No invented commitments | [Yes. No unsupported promises, deadlines, or guarantees were included.] |

## 6. Evaluation Framework

Each task should be reviewed against the following criteria.

| Criterion | Description | Result |
|---|---|---|
| Accuracy | Correct facts and calculations | [Pass – Calculations and classifications were verified.] |
| Clarity | Understandable language | [Pass – Outputs used simple, clear and professional language.] |
| Instruction Following | Compliance with requirements | [Pass – Word limits, categories and specified instructions were followed.] |
| Output Structure | Correct format | [Pass – Tables, bullet points and email formats were maintained.] |
| Responsible AI | Avoids unsupported claims | [Pass – Ambiguous cases were flagged and missing information was acknowledged.] |

**Important:** Record only actual experimental observations.

## 7. Repository Structure

```text
fintech-zero-shot-ai-assistant/
│
├── README.md
│
├── prompts/
│   ├── task-1-emi.md
│   ├── task-2-complaints.md
│   ├── task-3-summary.md
│   └── task-4-communication.md
│
├── results/
│   └── experiment-results.md
│
├── evaluation/
│   └── evaluation-log.md
│
├── screenshots/
│   └── README.md
│
└── reflection.md
```

## 8. Tools and Technologies

- Generative AI / Large Language Models
- Zero-Shot Prompt Engineering
- ChatGPT or equivalent AI tool
- Microsoft Excel or Google Sheets
- GitHub
- Markdown documentation

## 9. Responsible AI and Risk Management

This project follows these principles:

1. Use fictional customer data only.
2. Never publish banking credentials.
3. Verify numerical calculations independently.
4. Identify unsupported AI-generated claims.
5. Escalate ambiguous cases for human review.
6. Avoid making unverified financial commitments.
7. Preserve original experiment outputs.
8. Acknowledge AI assistance appropriately.

## 10. Limitations

- This is an academic prototype.
- No real banking systems are integrated.
- No live customer data is processed.
- No production deployment has been performed.
- Model performance may vary across tools and settings.
- Human verification remains necessary.

## 11. Future Scope

- Few-shot prompting experiments
- Automated complaint classification
- Structured JSON outputs
- Expanded synthetic datasets
- Prompt evaluation dashboards
- Human-in-the-loop review workflows

## 12. Reflection

**100-word reflection:**

[The biggest improvement came from adding clear instructions, specific constraints, and structured output requirements to my prompts. Initially, AI generated basic responses, but after refinement, the outputs became more accurate, organised, and relevant to FinTech business applications. Adding ambiguity-handling rules improved complaint classification, while independent calculations helped verify financial accuracy. I also learned that AI can make assumptions when information is incomplete, so prompts must clearly instruct it not to invent missing details. This project helped me understand that effective prompt engineering is not just about asking questions but about guiding, evaluating, and improving AI-generated results.]

## 13. Author

**Student Name:** [Avantika] 
**Student ID:** [2620992550]
**Program:** BBA FinTech  
**University:** Chitkara University

## 14. Academic Integrity

This repository documents educational AI experiments.

All results, screenshots, calculations, and evaluation findings must represent genuine work. AI-generated content should be reviewed and acknowledged according to university guidelines.
