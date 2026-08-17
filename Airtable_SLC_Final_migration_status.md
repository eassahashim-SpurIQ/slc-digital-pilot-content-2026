# Airtable SLC Final Migration Status

Base: SLC Final (`appOmGakTzgU2AEt3`)

## Completed

- Confirmed local Airtable MCP is working.
- Found base `SLC Final`.
- Kept `Target list` as the canonical table.
- Added `Priority` field to `Target list`.
- Merged priority/DNC logic into `Target list`:
  - 480 original target records read.
  - 108 priority target records read.
  - 55 do-not-contact records read.
  - 7 existing records updated in first merge pass.
  - 155 records created from priority/DNC tables.
  - 11 Veena removal variants corrected after brand-level pass.
- Final `Target list` record count: 635.

## Priority Distribution

- Blank: 471
- P0 - Do Not Contact: 62
- P1 - Consumer Wallets: 5
- P1 - SLC Priority: 14
- P2 - Institutional Wallet Infrastructure: 7
- P2 - SLC Priority: 4
- P3 - Wallet Infrastructure: 7
- P4 - Digital Asset Exchanges & Wallets: 19
- P5 - Institutional Digital Assets: 4
- P6 - UAE: 12
- P7 - Saudi Arabia: 4
- P8 - Bahrain: 2
- P9 - Asia-Pacific (Singapore): 10
- P9 - Asia-Pacific (Hong Kong): 4
- P9 - Asia-Pacific (Japan): 4
- P9 - Asia-Pacific (South Korea): 3
- P9 - Asia-Pacific (Australia): 3

## Veena Removal Handling

The following are now marked `P0 - Do Not Contact` in the canonical `Target list`, including company-name variants:

- Airwallex
- Payoneer
- Moneycorp
- Ebury
- 3S Money
- Tide
- MultiPass
- thinkmoney / Think Money
- DiPocket
- DFNS

## Tables Still Present

Airtable's `delete-table` tool is available, but it explicitly requires user confirmation before deletion. Tables still present:

- Overview
- Stage Plan
- Signals
- Final copies
- Signal Companies
- Priority Target List
- Target list
- Do not contact
- Sample Lead
- Segment Priority

## Pending Confirmation

To make the base contain only one table, delete every table except `Target list`.
