# Understanding Plasma, A Series

## Outline

- [Preface](0-preface.md)
- [Introduction](1-introduction.md)
- Basic concepts
  - Spend Transaction
  - Deposit
  - In-Flight Transaction
  - Competing Transactions / Competitors
  - Canonical Transaction
  - Exitable Transaction
  - Valid Transaction
  - [Merkle Trees](basic_concepts/merkle_tree.md)
  - UTXOs
  - RLP
  - Exit / Exit Bond
  - Piggyback / Piggyback Bond
  - Challenge Period
  - ...

- Desired Exit Mechanisms

Owner of input `in` of `tx` must prove:
1. `tx` is exitable.
2. `tx` is non-canonical.
3. `in` is not spent in any transaction other than `tx`.

Owner of output `out` of `tx` must prove:
1. `tx` is exitable.
2. `tx` is canonical.
3. `out` is not spent.

- How Plasma Works (happy paths)
  - Root chain
  - Child chain
  - New transactions
  - Exits
  - Challenge Period
- Faults and Mitigations (sad paths)
  - Block witholding
  - Faulty Exits
  - Invalid child block
  - ...
- Specifications
  - Plasma MVP
    - Single child chain
    - 2 inputs / 2 outputs
    - 14 day exit window
  - Plasma Cash
    - non-fungible
    - no confirmations
- Implementations
  - omisego/plasma-mvp
  - omisego/plasma-cash
