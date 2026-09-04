# 3. Protocol Architecture & Non-Custodial Infrastructure

Liquida Exchange operates as a decentralized autonomous protocol deployed across high-speed, low-fee Ethereum Virtual Machine (EVM) Layer-2 networks (such as Base and Arbitrum). By eliminating centralized intermediaries, the protocol ensures that users retain absolute cryptographic ownership of their funds at all times.

## 3.1 Core Participant Roles
* **Student Savers & Depositors:** Verified students who deposit local fiat converted to $LPUSD to protect purchasing power and earn organic baseline yields.
* **P2P Liquidity Facilitators:** Distributed network nodes managing local fiat gateways via GCash, Maya, MariBank, and GoTyme to clear micro-transfers instantly.
* **Protocol Liquidators:** Automated bots and actors monitoring collateral health factors ($HF < 1.0$) across debt positions to ensure systemic solvency.

## 3.2 Algorithmic Peg Mechanics
The stability of $LPUSD is maintained through an over-collateralized debt position (CDP) architecture combined with decentralized liquidity pools. When demand for $LPUSD rises, arbitrageurs mint new tokens at parity by locking approved collateral assets. Conversely, when market demand retracts, positions are repaid or liquidated, contracting supply and defending the $1.00 USD peg.

* **Mathematical Stability Model:** Let $C$ represent total locked crypto collateral value and $D$ represent minted $LPUSD debt. The protocol enforces a minimum collateralization ratio $CR_{min} = 150\%$. If $C / D < 1.10$, automated liquidation is immediately triggered.