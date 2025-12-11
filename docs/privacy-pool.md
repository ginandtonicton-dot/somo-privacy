# 🔒 ZK Privacy Pool

## Overview

The SOMO ZK Privacy Pool enables users to make private, untraceable transactions on Solana using Zero-Knowledge cryptography.

## How It Works

```
    DEPOSIT                         WITHDRAW
    
┌─────────────┐                ┌─────────────┐
│  Wallet A   │                │  Wallet B   │
│  (Public)   │                │   (New)     │
└──────┬──────┘                └──────▲──────┘
       │                              │
       │ 1. Deposit                   │ 4. Withdraw
       │    + Secret                  │    + ZK Proof
       │                              │
       ▼                              │
┌─────────────────────────────────────────────┐
│                                             │
│            SOMO Privacy Pool               │
│                                             │
│   2. Store commitment hash                  │
│   3. Break link between wallets             │
│                                             │
└─────────────────────────────────────────────┘
```

### Step-by-Step

1. **Generate Secret:** User creates a random secret locally
2. **Create Commitment:** Hash of secret becomes the "commitment"
3. **Deposit:** Send tokens + commitment to Privacy Pool
4. **Wait:** Tokens mix with other deposits (improves privacy)
5. **Withdraw:** Prove you know a valid secret (ZK proof) without revealing which deposit is yours
6. **Receive:** Tokens sent to new wallet with no traceable link

## Privacy Guarantees

| Feature | Description |
|---------|-------------|
| **Unlinkability** | No on-chain link between deposit and withdrawal |
| **Anonymity Set** | Privacy increases with more pool participants |
| **Non-Custodial** | Protocol never controls your funds |
| **Verifiable** | Anyone can verify proofs are valid |

## Contract Address

```
JAMD8qSDiLHoV3RqyKAUGy9n8J2r7GFVhkzogumMPh3w
```

[View on Solscan](https://solscan.io/account/JAMD8qSDiLHoV3RqyKAUGy9n8J2r7GFVhkzogumMPh3w)

## Fees

| Action | Fee | Destination |
|--------|-----|-------------|
| Deposit | 1.5% | Treasury |
| Withdraw | 0% | - |

*Fees support protocol development and buyback programs.*

## Privacy Tiers

Different deposit amounts for different needs:

| Tier | Amount | Use Case |
|------|--------|----------|
| Micro | 100 SOMO | Small transactions |
| Standard | 1,000 SOMO | Regular use |
| Large | 10,000 SOMO | Larger transfers |
| Whale | 100,000 SOMO | High-value privacy |

*More participants in each tier = stronger privacy*

## Best Practices

### Maximize Privacy

1. **Wait before withdrawing** - Let more deposits accumulate
2. **Use standard amounts** - Stick to tier amounts
3. **Fresh wallet** - Always withdraw to a new wallet
4. **Multiple withdrawals** - Split large amounts

### What NOT to Do

- ❌ Withdraw immediately after deposit
- ❌ Withdraw exact deposited amount (minus fees)
- ❌ Withdraw to a linked wallet
- ❌ Share your secret with anyone

## Technical Details

### Commitment Scheme

```
commitment = hash(secret || nullifier)
```

- **Secret:** Random 256-bit value (keep private!)
- **Nullifier:** Derived from secret, prevents double-spend
- **Commitment:** Stored on-chain, proves deposit exists

### ZK Proof

When withdrawing, user proves:
1. They know a secret corresponding to a valid commitment
2. The nullifier hasn't been used before
3. Without revealing which commitment is theirs

### Nullifier System

- Each deposit generates a unique nullifier
- Nullifier is revealed only at withdrawal
- Prevents using same deposit twice
- Doesn't reveal deposit-withdrawal link

## Integration

### For Developers

The Privacy Pool can be integrated into other applications:

```javascript
// Example: Check if nullifier is spent
const isSpent = await program.account.nullifier.fetch(nullifierPDA);
```

*Full SDK documentation coming in Phase 3*

## FAQ

**Q: Is my deposit safe?**
A: Yes, the protocol is non-custodial. Your tokens are secured by Solana blockchain.

**Q: Can anyone see my deposit?**
A: Deposits are visible on-chain, but withdrawals cannot be linked to deposits.

**Q: What if I lose my secret?**
A: You cannot recover your deposit. Keep your secret safe!

**Q: How long should I wait?**
A: Longer = better privacy. Minimum recommended: 24 hours.

**Q: Can the team see my transactions?**
A: No. Even the team cannot link deposits to withdrawals.

---

*Privacy is a fundamental right. SOMO makes it accessible on Solana.*
