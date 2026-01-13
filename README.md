# Solana Token Creation Guide (SPL Tokens)

This repository explains how Solana tokens are created, including minting,
metadata, supply configuration, and authority settings.

It is designed to support developers and no-code tools that act as a
Solana token creator, helping users understand the SPL token launch process.

---

## What Is a Solana Token?

A Solana token follows the SPL (Solana Program Library) standard.
It requires a mint account, metadata, and authority configuration.

---

## How a Solana Token Creator Works

A Solana token creator abstracts the SPL token minting process into a simple workflow.

Typical responsibilities include:
- Creating the mint account
- Setting token decimals and supply
- Uploading and linking metadata
- Revoking mint and freeze authority
- Confirming on-chain deployment

---

See `token-creator-checklist.md` for a full launch checklist.

## No-Code Token Creation

For users who do not want to use the Solana CLI or write scripts,
a no-code Solana token creator can handle the entire process via a web interface.

Example:
https://www.soltokenlaunch.com
