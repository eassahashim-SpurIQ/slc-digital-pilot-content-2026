# SLC File Cross-Check Against Email Direction

Date reviewed: 17 Aug 2026

## Source Instruction Used

Primary email instruction used for this cross-check:

- Veena Dandapani email, 6 Aug 2026, "Re: Next Steps and Discussion Document"

Core interpretation:

- Remove primarily B2B/payment-provider style accounts: Airwallex, Payoneer, Moneycorp, Ebury, 3S Money, Tide, MultiPass, thinkmoney, DiPocket.
- Add or prioritize consumer wallets, institutional wallet infrastructure, wallet infrastructure, digital asset exchanges/wallets, institutional digital assets, and crypto/digital banking targets across UAE, Saudi Arabia, Bahrain, Singapore, Hong Kong, Japan, South Korea, and Australia.
- DFNS is a special case: Veena wrote "DFNS (already have.. remove)", so it should not be treated as a new add.

## File-By-File Meaning

### 1. Target list 2-Grid view.csv

What it is:

- This is your working Signal List 2 / execution list.
- It has 550 companies and columns for company, domain, country/region, source/register, and signal buckets.
- Sources in this file include ESMA CASP register, FCA/Central Bank registers, EBA EUCLID, Veena's 6 Aug email, UK Gambling Commission register, and SLC/Hunter research ratings.

How it maps to the email:

- This is the closest file to the final target list you should work from.
- Veena's add list is covered here, except DFNS, which is correct because Veena said not to newly add DFNS.
- It includes 65 rows sourced directly from "Veena's email, 6 Aug 2026" and 19 rows marked as "Veena's email, 6 Aug 2026 + ESMA crypto licence register".

Important flags:

- It still has 2 remove-list style matches:
  - The ai Corporation Limited: this is likely connected to Airwallex and should be reviewed/suppressed.
  - PAYONE GmbH: this matched the Payoneer removal check, but this needs human review because PAYONE and Payoneer may not be the same company. Do not automatically delete it without checking.
- The exported CSV has empty values in the signal columns: Newly licensed Crypto, New wallet firms, Customer report, send codes by text, Hiring. The source/register column still carries most of the signal meaning.

Use this for:

- Main Airtable/Clay working list.
- Prioritization and campaign execution after the remove-list review.

Do not use this for:

- Do-not-contact storage. Removed companies should live in Do not contact only.

### 2. SLC - EMI PAYMENT WALLETS- 20270702-2.xlsx

What it is:

- This is an SLC-shared curated wallet/EMI lead sheet.
- It has 158 rows in one sheet named "Wallet Leads".
- Columns include Company, Country, Category, Website, key execs/founders, LinkedIn, Pilot Likelihood, Fraud Intensity, Telco Leverage, Public Fraud Signals, Relevant Public Reports, and Evidence Strength.

How it maps to the email:

- This supports SLC's wallet/payment-wallet direction, but it predates or does not fully reflect Veena's 6 Aug cleanup.
- It contains some companies Veena later asked to remove.

Remove-list hits found:

- DiPocket Limited
- 3S Money Club Limited
- MultiPass Platforms Limited
- Tide Platform Limited
- Airwallex

Use this for:

- Priority scoring reference.
- Fraud-intensity and telco-leverage context.
- Finding stronger first-batch accounts among wallet/neobank/payment-wallet firms.

Do not use this as:

- The final target list without suppression, because it still contains Veena-remove companies.

### 3. EMI List Paysafe-2.xlsx

What it is:

- This is a broad EMI/payment-registry universe.
- It has 7 sheets and 3,614 combined company rows across Europe, North America, Asia, Middle East, Africa, and South America.
- It includes regulator/source data such as licensedemis.com, FinCEN, FINTRAC, Central Bank sources, SAMA, CBUAE, CBB, and similar regional registers.

How it maps to the email:

- This is not a clean target list.
- It is a raw sourcing universe from which targets can be selected.
- It includes many pure EMI/B2B/payment-provider accounts, including accounts Veena explicitly removed.

Remove-list hits found:

- 134 remove-list matches across the workbook.
- Examples include DiPocket, 3S Money, Airwallex, Ebury, Moneycorp, MultiPass, Payoneer, Tide, and thinkmoney variants.

Use this for:

- Source/reference universe.
- Finding new EMI/payment companies only after filtering for wallet, crypto, fraud, identity, device-auth, or consumer-money-movement signals.

Do not use this as:

- A send-ready list.
- A priority list.

### 4. Outreach_Payments Wallets(Company Info).csv

What it is:

- This is an SLC/Hunter-style enriched outreach/company-info file.
- It has 119 companies and fields such as Website, Revenue, Employees, Type, Number of users, Average Balance, Any Fraud Recently?, Hunter's opinion, Hunter's rating, Authentication, and Authenticator.

How it maps to the email:

- It is useful as enrichment and prioritization context, especially around fraud, authentication, and outreach judgement.
- It overlaps heavily with the SLC EMI Payment Wallets sheet, so it appears to be related to the same SLC-shared target research/workstream.
- It also still contains companies Veena later asked to remove.

Remove-list hits found:

- Tide Platform Limited
- 3S Money
- DiPocket Group
- MultiPass

Use this for:

- Enrichment.
- Personalization notes.
- Validating authentication method and fraud pain.
- Hunter/SLC priority hints.

Do not use this as:

- The only target source or the final target table.

## Overlap Findings

Key overlaps found:

- Outreach Payments Wallets vs SLC EMI Payment Wallets: 87 overlapping companies.
- SLC EMI Payment Wallets vs EMI List Paysafe: 105 overlapping companies.
- EMI List Paysafe vs Target list 2 / Signal list: 339 overlapping companies.
- SLC EMI Payment Wallets vs Target list 2 / Signal list: 36 overlapping companies.
- Outreach Payments Wallets vs Target list 2 / Signal list: 26 overlapping companies.

What this means:

- EMI List Paysafe is the broad source universe.
- SLC EMI Payment Wallets is a curated SLC scoring sheet from that general wallet/payment universe.
- Outreach Payments Wallets is an enriched/company-info view for outreach decisions.
- Target list 2 is your current operational target list built from multiple sources and Veena's latest direction.

## Recommendation

Use Target list 2-Grid view.csv as the primary working target list.

Before sending:

1. Suppress/remove the clear Veena removal matches from Target list 2.
2. Review PAYONE GmbH manually before suppression because PAYONE may not be Payoneer.
3. Keep DFNS out of the target list unless SLC explicitly reverses Veena's note.
4. Use SLC - EMI PAYMENT WALLETS as the priority/scoring reference.
5. Use Outreach_Payments Wallets as enrichment for authentication, fraud, Hunter rating, and personalization.
6. Use EMI List Paysafe only as a source universe, not as a send-ready list.

Clean working hierarchy:

- Final execution list: Target list 2 / Airtable Target list - Clean.
- Suppression list: Do not contact table.
- Scoring context: SLC - EMI PAYMENT WALLETS.
- Enrichment context: Outreach_Payments Wallets.
- Raw source universe: EMI List Paysafe.

## Immediate Action Items

- Add The ai Corporation Limited to review/suppression because it matched the Airwallex removal logic.
- Manually check PAYONE GmbH before deciding whether it belongs in do-not-contact.
- Do not add DFNS as a target.
- When importing to Airtable, keep only true targets in Target list and move removed companies to Do not contact.
