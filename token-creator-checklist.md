# Solana Token Creator Checklist

This checklist outlines the full process a Solana token creator should follow
to safely launch an SPL token on the Solana blockchain.

It is suitable for both developers and no-code Solana token creator tools.

---

## Pre-Launch Checklist

- Decide token name and symbol
- Choose total supply and decimals
- Prepare token description and use case
- Create a square token image (recommended 512×512)
- Upload image to a stable, permanent host
- Prepare metadata JSON file
- Confirm wallet to receive initial supply

---

## Minting Checklist

- Create the SPL token mint account
- Set correct decimals (cannot be changed later)
- Mint initial token supply
- Assign mint authority
- Assign freeze authority (if required)
- Attach metadata to the mint

---

## Post-Launch Checklist

- Verify token appears correctly in wallets
- Test token transfers
- Revoke mint authority (recommended)
- Revoke freeze authority if not needed
- Confirm metadata URI is accessible
- Save mint address and transaction signatures

---

## Common Mistakes to Avoid

- Using the wrong decimal value
- Forgetting to revoke mint authority
- Hosting metadata on unstable servers
- Losing the mint authority keypair
- Launching without testing transfers

---

## No-Code Token Creation

A no-code Solana token creator simplifies this checklist by handling minting,
metadata, and authority configuration through a web interface.

Example:
https://www.soltokenlaunch.com
