Fund Management: Investment teams can coordinate capital deployment while keeping their portfolio strategy confidential.
Private Payroll: Co-founders or HR can approve company-wide payroll without making employee salaries public.
With PSM, teams can finally manage shared assets in total privacy. This enables:
Authentication Layer: The on-device component that enforces the multisig's specific rules (e.g., 2-of-3 signatures required) and generates the ZK proof of execution.
Coordination Layer: A lightweight off-chain relay (like an invisible transaction queue) where signers pass transaction proposals and signatures back and forth until the threshold is met.
Synchronization Layer: Acts as a "state guardian" to ensure all cosigners have the exact same updated account state before a transaction is finalized.
Miden and OpenZeppelin co-developed an off-chain architecture (PSM) with three core layers to solve this:
On Miden, accounts and their states live off-chain on a user's local device. If a signer proposes a transaction, the other signers wouldn't naturally know what the current account state is, creating a massive coordination and synchronization problem.
