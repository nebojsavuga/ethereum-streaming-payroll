# Robinhood Streaming Payroll Smart Contracts
This project implements a progressive smart contract system for continuous payroll streaming, inspired by Robinhood’s blockchain innovation initiative. The system enables real-time salary payments and transparent vesting schedules, moving away from traditional monthly payroll cycles.

## Features
### Phase 1: ETH Streaming

Create salary streams in ETH with customizable start/end times and amounts.
Recipients can withdraw accumulated ETH at any time during the stream.
No cancellation in this phase.

### Phase 2: ERC-20 Token Support & Cancellation

Streams can use any ERC-20 token (e.g., USDC, USDT).
Stream senders can cancel streams; recipients receive earned funds, and unvested funds return to the sender.

### Phase 3: NFT Trading

Each stream is represented as an ERC-721 NFT.
Streams (and their future payments) can be traded on NFT marketplaces.
NFT ownership determines who can withdraw from the stream.
Security
Reentrancy protection on withdrawals
Integer overflow/underflow checks
Access control for sensitive actions (e.g., cancellation)
Proper token handling and time validation

### Testing
Includes comprehensive tests for stream creation, withdrawals, token support, cancellation, and NFT trading.
