# MERC independent on-chain verification status

Updated: 2026-10-14

## Evidence status

This is an investigation status record, **not** a completed on-chain audit or proof of reserves.

The following identifiers are **preliminary, not owner-confirmed**:

- Proposed mint: `5K9waoBc12BwYdTcoRexMyPqfvHE8DkxRAu4DqWtpump`
- Proposed community rewards wallet: `9ELSKjoXqSRgK8ECYXyU51AX3bRj7vBKiA31iYVskW6S`

### Attempted independent lookup

On 2026-10-14, public web discovery was attempted for both exact addresses, followed by direct Solscan explorer lookups. The direct explorer pages did not return accessible account records in the research environment. Search results did not provide address-specific, independently verifiable account state or transaction signatures. **No live Solana RPC response was obtained.** No negative conclusion about the existence or balance of either account can be inferred from these access failures.

| Check | Finding |
| --- | --- |
| Mint account existence and owner program | Unverified |
| Supply and decimals | Unverified |
| Mint and freeze authorities | Unverified |
| Token-2022 extensions, if applicable | Unverified |
| Proposed rewards wallet SOL and MERC balances | Unverified |
| Other token accounts belonging to wallet | Unverified |
| Transfers, minting, burns, distributions | No transaction signatures independently verified |
| Treasury address and balance | Not disclosed or verified |
| Project control of addresses | Not established |
| Token locks and reserves | Not established |

### Project-stated figures versus observed balances

- Approximately **202,530,000 MERC** described as team-controlled (project statement).
- **100,000,000 MERC** designated within that amount for community rewards (project statement; about **49.38%** of the stated team allocation).
- No verified on-chain balances were available for reconciliation. **Do not interpret this as a zero balance or a proven shortfall.**
- Designation is not proof of segregation, custody, lockup, or completed distribution.

### Next evidence required

1. Owner confirms the exact official mint through an authenticated project channel.
2. Query Solana mainnet `getAccountInfo` and `getTokenSupply` for the mint; retain response, slot, UTC time, decimals, supply, owner program, and authority status.
3. Query `getBalance` and `getTokenAccountsByOwner` for the proposed wallet, across the applicable token programs; retain slot, UTC time, and token account addresses.
4. Review finalized signatures and parsed transactions for the mint and wallet; publish transaction signatures, slots, UTC timestamps, amounts, and classifications (mint, burn, transfer, distribution).
5. Confirm any treasury/rewards wallet ownership with safe signed-message proof and corroborating official disclosures; never disclose private keys or recovery phrases.
6. Reconcile verified balances and historical flows to allocations, with explicit treatment of exchange, liquidity-pool, program-controlled, or other third-party accounts.

### Public inspection links

- [Proposed mint on Solscan](https://solscan.io/token/5K9waoBc12BwYdTcoRexMyPqfvHE8DkxRAu4DqWtpump)
- [Proposed rewards wallet on Solscan](https://solscan.io/account/9ELSKjoXqSRgK8ECYXyU51AX3bRj7vBKiA31iYVskW6S)

These links are inspection targets, **not verification evidence**.

No custody, reserves, lockup, token supply, or distribution claim is independently substantiated by this record.
