# Understanding Plasma, A Series

## Outline

- [Preface](0-preface.md)
- [Introduction](1-introduction.md)
- Basic concepts
  - [Merkle Tree](basic_concepts/merkle_tree.md)
  - Hash
  - Operator
  - Fraud Proof
  - UTXOs
  - RLP
  - ...
- How Plasma Works (happy paths)
  - Root chain
  - Child chain
  - New transactions
  - Confirmation Signatures
  - Exits
    - Limbo Exits
  - Fast Withdrawals
- Faults and Mitigations (sad paths)
  - Data Availability
-   Block Witholding
  - Faulty Exits
  - Invalid transactions
  - Invalid child blocks
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
