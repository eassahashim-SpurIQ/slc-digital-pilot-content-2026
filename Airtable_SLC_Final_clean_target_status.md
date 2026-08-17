# Airtable SLC Final - Clean Target Table Status

Base: SLC Final (`appOmGakTzgU2AEt3`)

## New Table Created

Created a new table: `Target list - Clean` (`tblssFOoK0c06KJle`).

This table is separate from the existing `Target list`. The existing `Target list` was not deleted.

## User Rule Applied

- `Do not contact` records should remain only in `Do not contact`.
- `Priority Target List` should remain untouched.
- `Priority Target List` companies should be brought into the new target table if they are valid targets.
- Existing target records should remain targets only if they do not overlap with `Do not contact`.

## Do Not Contact Check

Checked `Do not contact` against Veena's remove list and DFNS.

Missing DNC records added: 0

## Clean Table Result

Final `Target list - Clean` record count: 566

Priority distribution:

- Blank: 466
- P1 - Consumer Wallets: 5
- P1 - SLC Priority: 12
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

## DNC Overlaps Removed From New Clean Table

Removed from `Target list - Clean` after validation:

- `Stripe Payments UK`, because `Stripe` exists in `Do not contact`.
- `Nubank Wallet`, because `Nubank` exists in `Do not contact`.

## Not Touched In This Cleanup

- `Priority Target List` was not modified.
- Current old `Target list` was not deleted.
- `Do not contact` was not changed because no missing Veena/DNC companies were found.
