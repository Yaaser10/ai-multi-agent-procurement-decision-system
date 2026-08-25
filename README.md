# AI Multi-Agent Procurement Decision System

A multi-agent AI system that compares vendors using deterministic weighted scoring, AI-powered procurement analysis, vendor risk assessment, recommendations, and human approval.

## Key Features

- Multi-vendor comparison
- Weighted decision scoring
- Price normalization
- Delivery performance scoring
- Quality and reliability evaluation
- AI procurement analysis
- Vendor risk assessment
- AI recommendation generation
- Human approval
- Final procurement report

## System Architecture

```text
Vendor Offers
     ↓
Python Scoring Engine
     ↓
Verified Vendor Ranking
     ↓
Procurement Analyst Agent
     ↓
Vendor Risk Agent
     ↓
Recommendation Agent
     ↓
Human Approval
     ↓
Final Procurement Report
```

## How It Works

1. Vendor offers are provided with price, quality, delivery time, reliability, and notes.
2. Python calculates normalized price and delivery scores.
3. A weighted score is calculated for every vendor.
4. Vendors are ranked using verified numerical results.
5. The Procurement Analyst Agent explains the main trade-offs.
6. The Vendor Risk Agent identifies potential risks.
7. The Recommendation Agent recommends the strongest vendor.
8. A human approves or rejects the recommendation.
9. The system generates a final procurement report.

## Decision Weights

```text
Price        35%
Quality      30%
Delivery     20%
Reliability  15%
```

## Weighted Scoring Formula

```text
Final Score =
Price Score × 35%
+
Quality Score × 30%
+
Delivery Score × 20%
+
Reliability Score × 15%
```

Python performs the calculations instead of relying on the AI model for numerical scoring.

## Agents

### Procurement Analyst Agent

Analyzes:

- Price position
- Quality
- Delivery speed
- Reliability
- Vendor trade-offs

### Vendor Risk Agent

Identifies realistic procurement risks and classifies them as:

```text
LOW
MEDIUM
HIGH
```

### Recommendation Agent

Uses:

- Verified Python ranking
- Procurement analysis
- Vendor risk analysis

to recommend the strongest vendor and an alternative option.

## Human-in-the-Loop

The AI does not make the final purchasing decision.

```text
AI Recommendation
       ↓
Human Approval
     /     \
APPROVE   REJECT
```

## AI + Python + Human Design

```text
Python
↓
Normalize
Calculate
Score
Rank

AI
↓
Analyze
Assess Risk
Explain
Recommend

Human
↓
Approve
Reject
Decide
```

## Important Principle

```text
Cheapest Vendor ≠ Best Vendor
```

A procurement decision should consider multiple factors instead of price alone.

## Example Vendors

```text
Vendor A
Price: 85,000
Quality: 92
Delivery: 12 days
Reliability: 90

Vendor B
Price: 72,000
Quality: 78
Delivery: 8 days
Reliability: 72

Vendor C
Price: 79,000
Quality: 88
Delivery: 6 days
Reliability: 85
```

## Final Report Structure

```text
1. Decision Weights
2. Verified Vendor Ranking
3. Procurement Analysis
4. Vendor Risk Analysis
5. AI Recommendation
6. Human Decision
```

## Tech Stack

- Python
- Groq API
- Qwen
- Google Colab
- Multi-Agent Architecture
- Weighted Decision Scoring
- Procurement Analysis
- Risk Assessment
- Human-in-the-Loop AI
- Secure API Key Management

## What I Learned

This project demonstrates:

- Multi-criteria decision making
- Weighted scoring
- Deterministic vendor ranking
- AI-assisted procurement analysis
- Risk assessment
- Trade-off analysis
- Human approval workflows
- Separation between numerical calculations and AI reasoning

## Project Purpose

This project explores how deterministic Python calculations, specialized AI agents, and human oversight can collaborate to support structured procurement decisions.
