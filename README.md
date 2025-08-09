IFRS 17 Life Valuation Model - Excel Workbook

Overview

- Purpose: A compact and transparent IFRS 17 valuation model built in Excel. It demonstrates end to end cash flow projection, discounting, present values, and CSM mechanics in a way that is easy to review and audit.
- Audience: Recruiters and actuarial hiring managers who want to see practical IFRS 17 modelling skills with clear documentation and clean structure.
- File: mini_ifrs17_engine_uk.xlsx (no macros, works in standard Excel).

What It Demonstrates

- IFRS 17 mechanics: Builds fulfilment cash flows from projected cash flows and discount factors, then rolls forward the Contractual Service Margin using coverage units.
- UK context: Uses common UK actuarial conventions for discounting and projection.
- Rate modelling: Includes a CIR (Cox Ingersoll Ross) sheet to illustrate yield curve dynamics and discount factor construction.
- Auditability: All calculations are visible and traceable in the workbook with no hidden code.

Workbook Structure (key tabs)

- Setup: Centralised inputs and high level assumptions. Product settings, cohort and coverage units settings, timing conventions, and any initial balances. Start here to control a run.
- CIR: Interest rate model assumptions (kappa, theta, sigma, r0) and curve generation to produce a discount term structure consistent with UK practice. Includes discount factors derived from the curve.
- Projection: Deterministic policy cash flows over time. Premiums, claims, expenses, and acquisition costs aligned to cohorts and coverage units.
- Discount: Builds discount factors and zero rates from the CIR output and aligns them to projection periods.
- PV: Present value layer that converts nominal projected cash flows into discounted values used to compute fulfilment cash flows.
- CSM: Contractual Service Margin calculations and roll forward, including unlocking for changes in estimates if applicable and recognition over coverage units.

How To Use

1. Open mini_ifrs17_engine_uk.xlsx in Excel on Windows or Mac.
2. On Setup, set timing, cohort settings, coverage units, and any initial balances.
3. On CIR, adjust kappa, theta, sigma, and r0 to generate a curve and review discount factors.
4. Review Projection to validate premiums, claims, and expenses profiles.
5. Check Discount and PV to confirm discount factors apply correctly and PVs reconcile to expectations.
6. Inspect CSM to review recognition over coverage units and how changes flow through to profit emergence.

Notes and Scope

- Scope: Focused on GMM or BBA mechanics for a simple product to keep the model compact and easy to audit.
- Risk Adjustment: Not explicitly modelled as a separate tab in this build. It can be layered in later if needed.
- Unit of account: Illustrates a single portfolio or cohort setup and can be extended to multiple cohorts.
- Data: Uses toy example inputs and contains no client or confidential data.

What To Review (for recruiters)

- Structure: Clear separation between inputs, projection, discounting, PV, and CSM layers.
- Controls: Centralised assumptions on Setup make scenario testing quick and repeatable.
- Transparency: No VBA or macros. Reviewers can trace formula chains end to end.
- Presentation: Each sheet is labelled and laid out for easy audit. Headers and sectioning clarify purpose and flow.

Possible Extensions

- Add Risk Adjustment using a cost of capital approach and integrate it into fulfilment cash flows.
- Multi cohort support with aggregation and cohort level CSM.
- Sensitivity manager for rates, lapses, and expenses with side by side result comparison.
- Reconciliation dashboard with waterfalls for PV and CSM movements period over period.
- Data import from CSV to support larger scenarios reproducibly.

Repository Contents

- mini_ifrs17_engine_uk.xlsx - The Excel model.
- README.md - This documentation.

Why This Matters

- IFRS 17 requires clean separation of projected cash flows, discounting, and earnings recognition via CSM. This workbook shows the ability to design that structure clearly, build realistic discounting from a rate model such as CIR, and present results a reviewer can trust.

Contact

- Author: Divyanshi Verma (GitHub: @divvrma)
- Questions or feedback: Please open a GitHub issue or contact me via my profile.
