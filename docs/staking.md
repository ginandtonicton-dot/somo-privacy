# 💰 SOMO Staking

## Overview

Stake your SOMO tokens to earn passive rewards and gain governance voting rights.

## Staking Parameters

| Parameter | Value |
|-----------|-------|
| **APY** | 10% |
| **Reward Pool** | 250,000,000 SOMO |
| **Minimum Stake** | No minimum |
| **Lock Period** | None (flexible) |
| **Unstake Fee** | 2% |

## Contract Address

```
9PSRymTJrMFRFjyhy3j4g3FGY4t3czPcGLEiD3vPuhth
```

[View on Solscan](https://solscan.io/account/9PSRymTJrMFRFjyhy3j4g3FGY4t3czPcGLEiD3vPuhth)

## How Staking Works

```
┌─────────────┐         ┌─────────────────┐
│             │  Stake  │                 │
│   Wallet    │────────►│  Staking Pool   │
│             │         │                 │
└─────────────┘         └────────┬────────┘
       ▲                         │
       │                         │
       │    Rewards (10% APY)    │
       └─────────────────────────┘
```

### Step-by-Step

1. **Stake:** Deposit SOMO tokens into staking contract
2. **Earn:** Rewards accumulate every block (~400ms on Solana)
3. **Claim:** Withdraw rewards anytime
4. **Unstake:** Withdraw principal (2% fee applies)

## Reward Calculation

Rewards are calculated based on:

```
Daily Reward = (Staked Amount × APY) / 365

Example:
- Staked: 10,000 SOMO
- APY: 10%
- Daily Reward: (10,000 × 0.10) / 365 = 2.74 SOMO
- Monthly Reward: ~82 SOMO
- Yearly Reward: 1,000 SOMO
```

## Reward Sustainability

| Metric | Value |
|--------|-------|
| Total Reward Pool | 250,000,000 SOMO |
| Current APY | 10% |
| Estimated Duration | 5+ years |

*Treasury buybacks may replenish reward pool, extending duration*

## Governance Rights

Staking SOMO grants voting power:

| Staked Amount | Rights |
|---------------|--------|
| Any amount | Vote on proposals |
| 10,000+ SOMO | Create proposals |

See [Governance Documentation](governance.md) for details.

## Fees

| Action | Fee | Destination |
|--------|-----|-------------|
| Stake | 0% | - |
| Claim Rewards | 0% | - |
| Unstake | 2% | Treasury |

*Unstake fee prevents short-term farming and supports protocol*

## Staking Strategies

### Long-Term Holder
- Stake all tokens
- Compound rewards periodically
- Vote on governance proposals

### Active Trader
- Stake portion of holdings
- Keep some liquid for trading
- Claim rewards regularly

### Governance Participant
- Stake 10,000+ SOMO
- Create improvement proposals
- Lead community initiatives

## Benefits of Staking

| Benefit | Description |
|---------|-------------|
| **Passive Income** | 10% APY on staked tokens |
| **Governance** | Vote on protocol decisions |
| **Support Protocol** | Reduces circulating supply |
| **No Lock** | Unstake anytime |

## Risks

| Risk | Mitigation |
|------|------------|
| Smart Contract | Audits planned, non-custodial design |
| Token Price | Diversify, stake what you can afford |
| Unstake Fee | Plan for 2% fee when unstaking |

## FAQ

**Q: Is there a minimum stake?**
A: No, you can stake any amount of SOMO.

**Q: How often can I claim rewards?**
A: Anytime! Rewards accumulate continuously.

**Q: Is there a lock period?**
A: No, but there's a 2% unstake fee.

**Q: Can I stake from any wallet?**
A: Yes, any Solana wallet (Phantom, Solflare, etc.)

**Q: Where do rewards come from?**
A: From the 250M SOMO Staking Rewards allocation.

**Q: What happens when reward pool empties?**
A: DAO will vote on sustainability measures (buybacks, adjusted APY, etc.)

---

*Stake SOMO, earn rewards, shape the future of private DeFi.*
