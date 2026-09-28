# Codama Homework Notes

## Versions

- Anchor CLI: 1.1.2
- Node: v26.8.1
- Codama CLI: 1.6.3
- @codama/renderers-js: 2.5.0
- @solana/kit: 8.3.0

## TODO 3 — Account Resolution

`contributorAccount` and `contributorAta` can be derived because their seeds use values already available from the instruction inputs, while `tokenProgram` has a fixed known address.

`fundraiser` and `vault` must be provided because their derivation depends on values stored inside the Fundraiser account data (`fundraiser.maker` and `fundraiser.mintToRaise`), which Codama cannot know from the instruction inputs alone.
