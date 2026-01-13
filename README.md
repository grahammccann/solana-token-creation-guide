# Solana Token Creation Guide (SPL Tokens)

This repository explains how Solana tokens are created, including minting,
metadata, supply configuration, and authority settings.

It is designed to support developers and no-code tools that act as a
Solana token creator, helping users understand the SPL token launch process
before deploying a token on-chain.

---

## How Solana Tokens Are Created (Overview)

Creating a Solana token follows a defined sequence using the SPL Token program.

1. **Mint account creation**  
   A new mint account is created on-chain. This account defines the token itself,
   including the number of decimals and the authorities that control it.

2. **Supply configuration**  
   The creator decides whether to mint an initial supply immediately or mint
   tokens over time. Supply is controlled by the mint authority.

3. **Metadata attachment**  
   Token metadata such as name, symbol, description, and image is stored off-chain
   and linked to the mint using the Metaplex metadata standard.

4. **Authority management**  
   Mint and freeze authorities determine who can create new tokens or freeze
   balances. These authorities can be revoked to make the token immutable.

5. **On-chain confirmation**  
   Once transactions are confirmed, the token becomes visible in wallets and
   explorers and can be transferred like any other SPL token.

---

## What Is an SPL Token?

An SPL token is Solana’s standard for fungible tokens, similar in concept to
ERC-20 tokens on Ethereum.

Each SPL token consists of:
- A mint address
- A defined number of decimals
- One or more authority roles
- Optional metadata for wallets and explorers

---

## How a Solana Token Creator Works

A Solana token creator abstracts the SPL token minting process into a simplified
workflow, usually through a script or web interface.

Typical responsibilities include:
- Creating the mint account
- Setting token decimals and supply
- Uploading and linking metadata
- Minting the initial supply
- Revoking mint and freeze authority
- Confirming on-chain deployment

---

## Common Mistakes When Launching Tokens

- Using the wrong decimal value
- Forgetting to revoke mint authority
- Hosting metadata on unstable servers
- Losing access to the authority wallet
- Launching without testing transfers

---

## Token Launch Checklist

A full step-by-step checklist is available here:

See `token-creator-checklist.md` for the complete Solana token launch checklist.

---

## No-Code Token Creation

For users who do not want to use the Solana CLI or write scripts, a no-code
Solana token creator can handle minting, metadata, and authority configuration
through a web interface.

Example:
https://www.soltokenlaunch.com

---

## Further Reading

- Solana Program Library (SPL) Token documentation
- Metaplex Token Metadata standard
