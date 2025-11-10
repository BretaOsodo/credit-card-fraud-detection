# credit-card-fraud-detection

A sophisticated machine learning system for detecting fraudulent credit card transactions. This project implements a precision-optimized two-stage detection approach that reduces false positives by 73% while maintaining effective fraud detection capabilities.

## Business Impact Analysis
  ####Major Operational Improvement
  
  1. 73% Fewer False Alerts - Dramatically reduces manual review workload
  2. 29.5% Higher Precision - More accurate fraud detection
  3. 13.4% Better F1-Score - Improved overall balance
  4. 12,469 Fewer False Positives - Significant cost savings

## Cost-Benefit Tradeoff

While the two-stage system reduces recall, it provides substantial business benefits:
*Fewer legitimate transactions blocked → Better customer experience
*Reduced investigation costs → Higher operational efficiency
*More focused fraud team → Better resource allocation

##System Architecture
Precision-Optimized Two-Stage Framework.

graph TD
    A[Transaction Data] --> B[Stage 1: XGBoost Screener]
    B -->|Balanced Detection| C[Suspicious Transactions]
    B -->|Auto-approve| D[Legitimate Transactions]
    C --> E[Stage 2: Precision Filter]
    E -->|High Precision| F[Confirmed Fraud]
    E -->|Clear| G[73% Fewer False Alerts]
    F --> H[Focused Investigation]
