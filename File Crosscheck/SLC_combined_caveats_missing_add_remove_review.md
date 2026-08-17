# SLC Combined Caveats, Missing Items, Add/Remove Review

Date reviewed: 17 Aug 2026

Sources reviewed together:

- Fireflies task extraction: `SLC_all_meetings_task_extraction.md`
- Email task extraction: `SLC_email_trails_important_notes_and_task_extraction.md`
- Account discovery note: `SLC_account_discovery_from_emails_and_transcripts.md`
- File cross-check: `SLC_file_crosscheck_against_email.md`
- `Target list 2-Grid view.csv`
- `SLC - EMI PAYMENT WALLETS- 20270702-2.xlsx`
- `EMI List Paysafe-2.xlsx`
- `Outreach_Payments Wallets(Company Info).csv`

## Bottom Line

The working direction is correct: the campaign should focus on wallets, digital assets, crypto exchanges, wallet infrastructure, mobile/device authentication, fraud/account takeover, and regulated money movement where SLC has a real device-authentication reason to matter.

The main caveat is that the older SLC-shared files are not fully aligned with Veena's later 6 Aug 2026 correction. They should be used as evidence/enrichment sources, not as final target lists.

## What Looks Correct

- `Target list 2-Grid view.csv` is the right primary working target list.
- Veena's add list is covered in the current target CSV.
- DFNS is not missing from the target list, because Veena wrote "DFNS (already have.. remove)"; it should not be newly added.
- The campaign direction has correctly moved away from generic fintech and toward wallet/digital-asset/device-authentication accounts.
- The Airtable structure should keep Target list and Do not contact separate.

## Biggest Caveats

### 1. The Signal Columns Are Empty In The Export

In `Target list 2-Grid view.csv`, the signal columns are empty:

- Newly licensed Crypto
- New wallet firms
- Customer report
- send codes by text
- Hiring

The `Source / register` column still shows why many rows exist, but for SLC review this is not enough. SLC asked for signal-led targeting, not just a register list.

What this means:

- Before sending, each priority row should have at least one visible signal reason.
- A row sourced only from FCA/EBA/national EMI registers is weaker unless supported by wallet, crypto, fraud, customer complaint, SMS/text-code, hiring, product launch, or regulatory movement evidence.

### 2. The Broad EMI Register Rows Are Risky If Used Without Extra Signal Proof

The target CSV has 317 broad register-source rows from FCA/Central Bank/EBA/national e-money sources.

These are not automatically wrong, but they are not automatically SLC-fit either. Many may be pure EMI/payment infrastructure companies, which is exactly the category Veena pushed away from.

Keep them only when the company has:

- consumer wallet or app-based money movement
- crypto/digital asset activity
- user/customer authentication flow
- SMS/text-code weakness
- fraud/account-takeover/customer complaint evidence
- recent identity/fraud/security/compliance hiring
- relevant regulatory deadline or newly licensed status

### 3. Older SLC Files Still Contain Veena-Remove Companies

The SLC-shared EMI and outreach files contain companies Veena later said to remove:

- Airwallex
- 3S Money
- Tide
- MultiPass
- Think Money / thinkmoney
- DiPocket

So the SLC files should not be imported blindly.

### 4. Some High-Scoring SLC-Shared Companies Are Not In Target List 2

This is the biggest "missing" issue. Veena's explicit email list is covered, but SLC's own curated/enriched files contain additional high-signal wallet companies that are not in the current target CSV.

## Remove / Suppress / Review

### Add To Do Not Contact Or Suppression

If not already present, add these:

- Think Money Limited / thinkmoney
- Airwallex and known Airwallex entities
- 3S Money / 3S Money Club Limited
- Tide / Tide Platform Limited
- MultiPass / MultiPass Platforms Limited
- DiPocket / DiPocket Limited / DiPocket Group
- Moneycorp
- Ebury
- Payoneer
- DFNS as duplicate/remove, not as a new target

Additional non-Veena suppression from SLC files:

- Guavapay: the outreach file says "DO NOT REACH OUT - Company in liquidation".

### Current Target List Rows To Review

Only two direct review/suppression matches were found in `Target list 2-Grid view.csv`:

- The ai Corporation Limited, domain `aicorporation.com`: review as likely Airwallex-related / remove-style match.
- PAYONE GmbH, domain `payone.com`: review manually. It matched Payoneer logic loosely, but PAYONE and Payoneer may not be the same company.

## Companies To Add To Target List

Veena's explicit add list is already covered. The additional add candidates below come from SLC-shared scoring/enrichment files and are missing from Target list 2.

### Strong Add Candidates From SLC EMI Payment Wallets

Add or review-add these first because they scored high for pilot likelihood, fraud intensity, telco leverage, or evidence strength:

- MuchBetter, `muchbetter.com` - gaming wallet, high fraud intensity.
- Onyze, `onyze.com` - institutional crypto wallet/custody, high fraud intensity.
- e& money, `eand.com` - UAE telco wallet, high telco leverage.
- STC Pay, `stcpay.com` - Saudi telco wallet, high telco leverage.
- Ooredoo Money Qatar, `ooredoo.qa` - telco wallet, high telco leverage.
- Ooredoo Money Kuwait, `ooredoo.com.kw` - telco wallet, high telco leverage.
- Careem Pay, `careem.com` - UAE super-app wallet.
- GrabPay, `grab.com` - Singapore super-app wallet.
- Bnext, `bnext.es` - Spain neobank/stored-value wallet.
- Rebellion Pay, `rebellionpay.com` - Spain neobank wallet.
- N26, `n26.com` - Germany neobank wallet.
- Bunq, `bunq.com` - Netherlands neobank wallet.
- Hype, `hype.it` - Italy neobank wallet.
- YAP, `yap.com` - UAE neobank wallet.
- Nubank Wallet, `nubank.com` / `nubank.com.br` - Brazil neobank wallet.
- Ualá, `uala.com` - Argentina neobank wallet.

Hold / do not add unless confirmed active:

- Ziglu: the SLC file labels it "In receivership".

### Strong Add Candidates From Outreach Payments Wallets

These are not in Target list 2 and were marked as Hunter rating 1, "Reach out now", or connection-led:

- Coins.ph, `coins.ph` - Philippines wallet/payment app, SMS/biometric/PIN.
- GCash, `gcash.com` - Philippines market leader with visible fraud pressure.
- GrabPay, `grab.com` - also appears in SLC EMI scoring.
- Mercado Pago Mexico, `mercadopago.com.mx` - payment/e-commerce wallet with scam activity.
- OVO, `ovo.id` - Indonesia payment/super-app wallet.
- Nubank Wallet, `nubank.com.br` - also appears in SLC EMI scoring.
- Skrill Limited, `skrill.com` - payment/crypto/money transfer, TOTP/2FA.
- Circle UK Trading Limited, `circle.com` - crypto/stablecoin, hardware-key/TOTP context.

Review-add, but not first priority:

- Creditas, `creditas.com`
- Konfio, `konfio.mx`
- Neon, `neon.com.br`
- Yoco, `yoco.com`

Reason: they have Hunter/connection value, but they are less directly tied to Veena's explicit wallet/digital asset/regional priority than the first group.

Do not add to first wave despite Hunter rating:

- Stripe Payments UK Ltd: too much like broad payment infrastructure unless a very specific identity/attestation use case is identified.
- TrueLayer Limited: B2B/open banking infrastructure; keep for later only if SLC wants an infrastructure wave.

## What May Be Wrong Or Incomplete

1. Treating any register row as "signal-qualified" without evidence is too weak for SLC's stated expectation.
2. Using the SLC EMI or Outreach files directly would reintroduce companies Veena asked to remove.
3. The current target CSV does not visibly show the signal evidence columns populated, which weakens the story to SLC.
4. Do not contact should include both Veena removals and operational no-go statuses such as Guavapay liquidation.
5. PAYONE GmbH needs manual verification before removal.
6. Some strong SLC-shared wallet candidates are absent from the current target list and should be added or at least reviewed.

## Recommended Next Step

Create three statuses in Airtable:

- `Target`: clean target, can be worked.
- `Review`: unclear fit, domain/entity ambiguity, or needs proof.
- `Suppress`: Veena remove, duplicate, liquidation, receivership, or not first-wave fit.

Then:

1. Move Veena removals and Guavapay to `Suppress`.
2. Move PAYONE GmbH to `Review`.
3. Add the strong SLC EMI wallet candidates above to `Target` or `Review`.
4. For broad FCA/EBA/register rows, keep only the rows with visible signal proof.
