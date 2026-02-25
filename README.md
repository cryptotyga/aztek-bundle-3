Fund Management: Investment teams can coordinate capital deployment while keeping their portfolio strategy confidential.
Private Payroll: Co-founders or HR can approve company-wide payroll without making employee salaries public.
With PSM, teams can finally manage shared assets in total privacy. This enables:
Authentication Layer: The on-device component that enforces the multisig's specific rules (e.g., 2-of-3 signatures required) and generates the ZK proof of execution.
Coordination Layer: A lightweight off-chain relay (like an invisible transaction queue) where signers pass transaction proposals and signatures back and forth until the threshold is met.
Synchronization Layer: Acts as a "state guardian" to ensure all cosigners have the exact same updated account state before a transaction is finalized.
Miden and OpenZeppelin co-developed an off-chain architecture (PSM) with three core layers to solve this:
On Miden, accounts and their states live off-chain on a user's local device. If a signer proposes a transaction, the other signers wouldn't naturally know what the current account state is, creating a massive coordination and synchronization problem.
On Ethereum (e.g., Safe) or Solana (e.g., Squads), multisigs are easy because everyone can look at the public ledger to see the current balance, who has signed, and what the proposed transaction is.
The Problem: Privacy Breaks Coordination
The article explains how Miden, in partnership with OpenZeppelin, solves the unique challenge of building a multi-signature (multisig) wallet on a privacy-by-default blockchain. In traditional blockchains, multisigs rely on public transparency so all signers can see the exact same state and transaction. Because Miden stores account state locally and privately, signers could easily fall out of sync. To fix this, Miden introduces Private State Management (PSM), an off-chain coordination system that ensures all signers stay synchronized on the latest private state without exposing their data to the public network.
Privacy infrastructure doesn't matter if everyday people can't use the apps. This is how we bring real-world finance on-chain.
