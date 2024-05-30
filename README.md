# catofftask
Rust-based smart contract using the Anchor framework to mint a new SPL token and transfer it bw two accounts
# Solana SPL Token Smart Contract

This is a simple Solana smart contract written in Rust using the Anchor framework. It allows you to mint a new SPL token and transfer tokens between accounts.

## Prerequisites

Before you begin, ensure you have the following installed:

- [Rust](https://www.rust-lang.org/tools/install)
- [Solana CLI](https://docs.solana.com/cli/install-solana-cli-tools)
- [Anchor CLI](https://project-serum.github.io/anchor/getting-started/installation.html)

## Setup

1. Clone this repository:

```bash
git clone https://github.com/your-username/solana-spl-token-contract.git
cd solana-spl-token-contract

Install the project dependencies:

bash
codecargo install --json=1 anchor-cli --locked
Deployment

Start a local Solana testnet:

bash
codesolana-test-validator

In a new terminal window, navigate to the project directory and deploy the smart contract:

bash
codeanchor build
anchor deploy

This will build the smart contract and deploy it to the local testnet. Make sure to keep the test validator running in the other terminal window.
Testing
After deploying the smart contract, you can test its functionality using the Solana CLI and the Anchor client.

In a new terminal window, navigate to the project directory.
Mint a new SPL token:

bash
 codeanchor run mint-token --amount 1000
This will mint 1000 tokens to a new account.

Transfer tokens between accounts:
anchor run transfer-token --amount 500
