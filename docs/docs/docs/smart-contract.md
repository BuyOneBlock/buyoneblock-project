# 🧾 Smart Contract — 1BONEBU Utility Token

This document describes the core logic, roles, and design principles of the 1BONEBU smart contract, in alignment with the Whitepaper 1.0, Whitepaper 2.0, and the Utilities & Access model.

The 1BONEBU token is a **utility token** designed for **access**, not ownership or financial returns.

---

## 1. Contract overview

- **Name:** Buy One Block Utility  
- **Symbol:** 1BONEBU  
- **Type:** Utility token  
- **Standard:** BEP‑20 / ERC‑20 compatible (depending on deployment chain)  
- **Use case:** Access to utilities and opportunities managed by the Buy One Block Holding

The contract is designed to be:

- simple,  
- auditable,  
- secure,  
- fully aligned with the holding‑controlled model.

---

## 2. Design principles

The 1BONEBU contract is built around the following principles:

- **Utility, not equity:**  
  The token does not represent shares, dividends, or ownership of any asset.

- **Access, not investment:**  
  Holding the token provides **access to utilities and opportunities** managed by the holding — not direct participation in investments.

- **Centralized governance via the holding:**  
  Administrative rights are held by the **Buy One Block Holding** (or an address it controls).

- **Compliance & control:**  
  The contract avoids features that could be misinterpreted as financial promises or yield mechanics.

---

## 3. Core features

The 1BONEBU contract typically includes:

- **Standard transfers:**  
  Token holders can send and receive tokens like any standard BEP‑20/ERC‑20 token.

- **Fixed or capped supply (according to tokenomics):**  
  Total supply is defined and published in the tokenomics documentation.

- **Ownership / Admin role:**  
  A privileged role (the holding) with limited, clearly defined powers.

- **No automatic rewards or reflections:**  
  No on‑chain yield, no reflection, no auto‑distribution, no auto‑staking.

- **No direct link to investments:**  
  The contract does not track or represent company assets or investment performance.

---

## 4. Roles & governance

### 4.1 Contract owner / admin

- **Entity:** Buy One Block Holding (or a wallet it controls)  
- **Powers (example, depending on final implementation):**
  - update specific configuration parameters,  
  - manage access lists if needed (for compliance),  
  - pause certain functions in case of emergency (optional),  
  - manage treasury or company‑owned wallets.

The owner **does not**:
- grant direct ownership of assets,  
- distribute profits from investments via the contract,  
- create any financial rights for holders.

### 4.2 Token holders

Token holders:

- hold 1BONEBU as a **utility token**,  
- can transfer, receive, and hold tokens,  
- may qualify for access to utilities, programs, and opportunities defined off‑chain by the holding,  
- do **not** gain any ownership, voting rights in the company, or claims on assets.

---

## 5. Alignment with Utilities & Access

The smart contract is intentionally **minimalist and compliant**.  
All **utilities and access** are defined and managed **off‑chain** by the Buy One Block Holding, based on:

- the amount of tokens held,  
- the holding duration,  
- compliance checks,  
- internal rules of the holding.

The on‑chain contract:

- confirms balances,  
- enforces transfers,  
- ensures transparency and traceability.

The off‑chain governance:

- decides which holders gain access to which utilities or opportunities,  
- applies eligibility criteria,  
- manages real‑estate and business operations.

👉 **The holding manages — the token proves access eligibility.**

---

## 6. Risk & compliance considerations

To support a compliant structure:

- No promises of profit or yield are coded into the contract.  
- No direct revenue distribution mechanism is implemented.  
- No token function automatically links holdings to company investments.

The contract is a **technical representation of a utility token**, not a financial product.

---

## 7. Future upgrades

Depending on the roadmap, future iterations may introduce:

- optional role‑based access control extensions,  
- upgradeability via a proxy pattern (if chosen),  
- integrations with KYC/eligibility systems (off‑chain),  
- additional utility layers (within the bounds of compliance).

Any evolution will remain aligned with:

- Whitepaper 1.0 (Web3 utility),  
- Whitepaper 2.0 (holding + real‑estate access),  
- the Utilities & Access model,  
- the core principle: **access, not ownership.**

---

## 8. Disclaimer

The 1BONEBU smart contract:

- does not represent a share or equity,  
- does not guarantee returns,  
- does not grant ownership of any real‑estate or asset,  
- is a utility token contract used to identify holders for access purposes,  
in the context of the Buy One Block ecosystem governed by the holding.
