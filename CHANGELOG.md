
# Changelog

## v0.3.1
### Tokenomics
- **Pie Chart**: Fix wrong allocation for investors in the pie chart. 

## v0.3
### Architecture & Consensus
- **Consensus Mechanism Redesign**: Replaced the RSA-factoring "Shortcut Mining" with a **Poseidon2** hash-based PoW to optimize for ZK-proof compatibility.
- **Scaling PQC**: Renamed "Entangled Addresses" to **"Wormhole Addresses"** and upgraded the hash function to Poseidon2.
- **Removed Section**: The "Chain Interoperability" section (Hyperlane/Solana bridge) has been removed from this version.

### Tokenomics & Governance
- **Defined Supply**: Set a maximum supply of **21,000,000 coins**.
- **Reward Formula**: Implemented an exponentially decaying block reward heuristic ($block\_reward = (max\_supply - current\_supply) / constant$).
- **Allocations**:
    - **Investors**: 20-30% allocation, liquid from day one (replaces 4-year vesting).
    - **Company**: 50% of block rewards for the first ~4 years (~10% total supply).
    - **DAO**: Future treasury funded by redirected block rewards.
- **Fees**: Specified a 1% volume-based fee for reversed transactions and 0.1% for ZK transactions.

### Wealth Preservation
- **High-Security Accounts**: Replaced "Interceptor" terminology with **"Guardian"**.
- **Check-Phrases**: Added a 50,000 iteration KDF for increased security against rainbow table attacks.
- **Removed Section**: "Cross-Chain Asset Wrapping" has been removed.

### Roadmap & General
- **Roadmap Updates**: Added "Dirac Beta" (Poseidon2 integration) for Nov 2025; renamed/rescheduled ZK aggregation to "Fermi Upgrade" (Q2 2026).
- **Security Estimates**: Updated Shor’s algorithm qubit requirements to ~2,300 logical qubits and complexity to $O(n^3)$.
- **PQC Parameters**: Updated ML-DSA-87 signature and key size estimates.

## v0.2
- Initial post-quantum architecture using ML-DSA and ML-KEM.
- Introduced Entangled Addresses (ZK-scaling).
- Proposed RSA-based "Quantum Canary" consensus.
- Detailed reversible transactions and check-phrases.

## v0.1 (unavailable)
- Initial draft
- This version was not preserved and is no longer available
