# 🚀 Avalanche CLI & Smart Contracts Setup Guide

Welcome to the ultimate guide for setting up Avalanche CLI and deploying ERC20 and Vault smart contracts! Follow these steps to get your environment up and running and manage your tokens securely. 🌐

## 📦 Prerequisites

Before you begin, ensure you have:

- **Unix-based operating system** (Linux/macOS)
- **Internet connection**

## 📋 Avalanche CLI Setup

### 1. Install Avalanche CLI

Download and install the Avalanche CLI with:

```bash
curl -sSfL https://raw.githubusercontent.com/ava-labs/avalanche-cli/main/scripts/install.sh | sh -s
```

This command fetches and executes the installation script for the Avalanche CLI.

### 2. Update Your PATH

Add the CLI binaries to your PATH to make the `avalanche` command available globally:

```bash
export PATH=~/bin:$PATH
```

### 3. Create a New Subnet

Create a new subnet with:

```bash
avalanche blockchain create mySubnet
```

Replace `mySubnet` with your desired subnet name.

### 4. Deploy the Subnet

Deploy your newly created subnet using:

```bash
avalanche blockchain deploy mySubnet
```

This command deploys the subnet you created.

## 🔑 ERC20 & Vault Contracts

### ERC20 Token Contract

The ERC20 Token contract implements the ERC20 standard for fungible tokens on the Ethereum blockchain. It provides the foundation for creating, transferring, and managing tokens.

**Key Features:**
- Standard functions: `transfer`, `approve`, `transferFrom`, `balanceOf`, `allowance`
- Optional minting and burning
- Ownership control for token management

### Vault Contract

The Vault Contract securely manages ERC20 tokens. It allows for the safe deposit, withdrawal, and balance checking of tokens.

**Key Features:**
- Deposit ERC20 tokens
- Withdraw ERC20 tokens
- Query token balances

## 🎉 You're All Set!


You now have Avalanche CLI installed and configured, and your ERC20 and Vault contracts deployed. For further details, check out:

- [Avalanche CLI Documentation](https://docs.avax.network)
- [ERC20 Token Standard](https://eips.ethereum.org/EIPS/eip-20)
- [Vault Contract Best Practices](https://docs.openzeppelin.com/contracts/4.x/)

