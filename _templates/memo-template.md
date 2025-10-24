# Executive Memo – FX Receivable Exposure (Scenario 2: U.S. Pharmaceutical Exporter)

**To:** Chief Financial Officer  
**From:** [Your Name], Treasury Analyst  
**Date:** October 24, 2025  
**Subject:** Hedging Recommendation for Euro Receivable Exposure  

Our firm expects to receive a **€8,000,000 payment** from a European distributor in **one year**. The current **spot rate (EUR/USD)** is approximately **1.0850**, and the **one-year forward rate** is **1.0890**. This creates a **foreign-exchange (FX) receivable exposure**, since the U.S.-dollar value of this payment will depend on the euro’s exchange rate one year from now.

## Exposure and Risk
If the euro **depreciates** against the U.S. dollar, our **USD receipts will fall**, reducing reported revenue and potentially affecting R&D budgets or profit targets.  
For example, if EUR/USD declines from 1.0850 to 1.00, the euro receivable’s USD value would drop from **$8.68 million to $8.00 million**, a **$680 thousand loss** purely from FX movement.  
Given current global uncertainty—ECB rate policy shifts, U.S. dollar strength, and geopolitical risk—this exposure is material and worth hedging.

## Hedging Alternatives
| Hedge | Pros | Cons |
|-------|------|------|
| **Forward Contract** | Locks in a fixed rate (1.0890) and eliminates FX uncertainty. No upfront cost. | No participation if the euro appreciates. |
| **Money-Market Hedge** | Uses borrowing/lending to lock in future USD proceeds. Avoids forward-counterparty exposure. | Operationally complex; requires short-term funding. |
| **Option Hedge (EUR Put)** | Guarantees a minimum exchange rate while allowing upside if the euro strengthens. | Up-front premium cost ($0.021 per EUR). |

## Next Steps
In **Stages 2–3**, I will develop a **spreadsheet model** comparing unhedged, forward, money-market, and option outcomes under multiple EUR/USD scenarios.  
This will quantify expected USD proceeds, visualize risk, and recommend an optimal hedge ratio.

## Technical Specification
The Excel model will:
- **Inputs:** EUR receivable, spot rate, forward rate, interest rates (USD & EUR), option strike and premium  
- **Outputs:** USD proceeds for each strategy  
- **Formulas:**  
  - Forward = EUR × Forward rate  
  - Money Market = [(EUR / (1 + r EUR)) × Spot] × (1 + r USD)  
  - Option = MAX(Spot or Strike) × EUR – Premium  

## Prompt Engineering
> “Create an Excel model comparing FX hedging strategies (forward, money-market, and option) for a €8,000,000 receivable due in one year. Inputs: spot 1.0850, forward 1.0890, USD interest 4.5 %, EUR interest 3.0 %, and option premium $0.021. Calculate and summarize USD proceeds under each strategy and provide a sensitivity table for ±5 % EUR/USD changes.”


