# UBC_2026_Hackathon_Snippet

Live site: https://snippet-gamma.vercel.app (Arc testnet; free testnet USDC at faucet.circle.com)

Demo video: https://www.youtube.com/watch?v=BNFDRMR4Yuw

Contract: SnippetLicenses 0xfc6a8dd5569ff53ca64065fac5eb17677ad1fe20, verified on the Arc testnet explorer

The 3 clips: The Final Push (COD gameplay) · Clipping on the Blockchain (podcast, original) · Outgunned by Marshals (Valorant gameplay)

Snippet is an on-chain marketplace for licensing short moments from streams and podcasts in USDC. Buyers pick a clip and a license tier (**Editorial**, **Social**, or **Commercial**), pay in one transaction on **Arc testnet**, and receive a verifiable certificate tied to the exact file SHA-256 hash and transcript.

## What It Does
* **Quote Search & Synced Captions:** Search spoken words to jump straight to that moment in a clip, with word-by-word highlighted captions.
* **Instant Revenue Splits:** A single smart contract call atomically splits USDC payments between the creator (70%), contributor/producer (20%), and platform (10%).
* **Wallet or Passkey Checkout:** Pay with a standard browser wallet or a gas-sponsored passkey smart account (no wallet extension needed).
* **On-Chain Verification:** Generates a "Verified on Arc" license certificate and lets anyone verify a master video file's hash on `/check`.
* **Live Feed & Ops Automation:** Streams sales in real time to the homepage, posts Discord creator alerts, and feeds a Grok ops bot for payout summaries and clip submission reviews.

## Tech Stack
* **Blockchain & Smart Contracts:** Arc Testnet (USDC native gas), Solidity, Foundry (`0xfc6a8dd5569ff53ca64065fac5eb17677ad1fe20`)
* **Frontend & Web3:** Next.js (App Router, TypeScript), wagmi, viem, RainbowKit
