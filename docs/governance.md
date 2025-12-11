# 🏛️ DAO Governance

## Overview

SOMO is governed by its community through a decentralized autonomous organization (DAO). Token holders can propose and vote on protocol changes.

## Governance Contract

```
3wGPjF7imm93WHgSjUoiXqGAtWbhTJVPxkEB6SSLn7ou
```

[View on Solscan](https://solscan.io/account/3wGPjF7imm93WHgSjUoiXqGAtWbhTJVPxkEB6SSLn7ou)

## How Governance Works

```
┌─────────────┐     ┌─────────────┐     ┌─────────────┐     ┌─────────────┐
│   Propose   │────►│    Vote     │────►│   Execute   │────►│  Implement  │
│  (72 hrs)   │     │  (72 hrs)   │     │  (24 hrs)   │     │             │
└─────────────┘     └─────────────┘     └─────────────┘     └─────────────┘
      │                   │                   │
      │                   │                   │
      ▼                   ▼                   ▼
  Requires           Community            Time-locked
  10,000 SOMO        votes                execution
  staked             YES/NO               
```

## Governance Parameters

| Parameter | Value |
|-----------|-------|
| **Min Stake for Proposal** | 10,000 SOMO |
| **Voting Period** | 72 hours |
| **Execution Delay** | 24 hours |
| **Vote Options** | Yes / No / Abstain |

## Who Can Participate?

| Action | Requirement |
|--------|-------------|
| Vote on proposals | Hold any SOMO |
| Create proposals | Stake 10,000+ SOMO |
| Execute passed proposals | Anyone |

## Proposal Types

### Protocol Upgrades
- Smart contract updates
- New feature implementations
- Security improvements

### Treasury Management
- Buyback programs
- Marketing spending
- Partnership funding
- CEX listing fees

### Parameter Changes
- Staking APY adjustments
- Fee structure changes
- Governance rules updates

### Community Initiatives
- Airdrop campaigns
- Grant programs
- Ecosystem development

## Proposal Lifecycle

### 1. Discussion (Off-chain)
- Discuss ideas in Telegram/Discord
- Gather community feedback
- Refine proposal details

### 2. Submission (On-chain)
- Proposer stakes 10,000 SOMO
- Proposal submitted to governance contract
- 72-hour voting period begins

### 3. Voting
- Token holders vote Yes/No/Abstain
- Voting power = staked SOMO amount
- Results calculated at end of period

### 4. Execution
- If passed: 24-hour timelock
- Then anyone can execute
- Changes take effect on-chain

### 5. Implementation
- Protocol updates automatically
- Community notified
- Documentation updated

## Voting Power

Your voting power equals your staked SOMO:

```
1 SOMO staked = 1 vote

Example:
- Alice stakes 50,000 SOMO → 50,000 votes
- Bob stakes 10,000 SOMO → 10,000 votes
- Carol stakes 5,000 SOMO → 5,000 votes
```

## Treasury

### Treasury Address
```
AZPr5gShbwTL7Lw2pGLqqVvjHnuRyVuRyV
```

### Treasury Balance
- Initial: 150,000,000 SOMO (15%)
- Plus: Protocol fees accumulate

### Treasury Income Sources

| Source | Fee |
|--------|-----|
| Privacy Pool Deposits | 1.5% |
| Unstaking | 2.0% |
| Governance Claims | 1.0% |

### Treasury Uses

Decided by governance vote:

- 🔥 **Buyback & Burn** - Reduce supply
- 📈 **CEX Listings** - Exchange fees
- 🎯 **Marketing** - Growth initiatives
- 🤝 **Partnerships** - Strategic deals
- 🛠️ **Development** - Protocol upgrades
- 🎁 **Rewards** - Community incentives

## Governance Best Practices

### For Proposers
1. Discuss idea with community first
2. Provide clear rationale
3. Include implementation details
4. Consider potential risks
5. Be responsive to questions

### For Voters
1. Read proposals carefully
2. Consider long-term impact
3. Participate in discussions
4. Vote based on protocol benefit
5. Not just personal gain

## Safeguards

| Safeguard | Purpose |
|-----------|---------|
| Minimum stake | Prevents spam proposals |
| Time delay | Allows community review |
| On-chain execution | Transparent & verifiable |
| No admin keys | True decentralization |

## Example Proposals

### Example 1: Adjust Staking APY
```
Title: Reduce Staking APY to 8%
Rationale: Extend reward sustainability
Implementation: Update reward rate in staking contract
Vote: Yes (65%) / No (35%) → PASSED
```

### Example 2: Marketing Budget
```
Title: Allocate 10M SOMO for CEX Listing
Rationale: Increase accessibility and volume
Implementation: Transfer from Treasury
Vote: Yes (78%) / No (22%) → PASSED
```

### Example 3: New Privacy Feature
```
Title: Add Multi-Asset Privacy Pool
Rationale: Enable private swaps
Implementation: Deploy new contract
Vote: Yes (52%) / No (48%) → PASSED
```

## FAQ

**Q: Can I vote without staking?**
A: No, you must stake SOMO to vote.

**Q: What happens to failed proposals?**
A: Nothing changes. Proposer can resubmit modified version.

**Q: Can proposals be cancelled?**
A: Only by proposer before voting ends.

**Q: Is voting anonymous?**
A: No, votes are recorded on-chain for transparency.

**Q: How do I create a proposal?**
A: Stake 10,000+ SOMO, then use the governance interface.

---

*Your voice matters. Shape the future of SOMO Privacy.*
