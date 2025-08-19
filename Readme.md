Deployed Contract Address = ST3WS0T17AP8FMT7NXC6J6FWJH5X5QFPAVHBPY5N1.nft-tree

🪙 Simple Token + NFT Counter (Stacks / Clarity)
📜 Overview

This is a minimal Clarity smart contract designed to deploy easily on Stacks with Clarinet.

It provides:

A basic fungible token (FT)

A basic non-fungible token (NFT)

A simple counter variable for testing

Perfect for learning, demos, or boilerplate for bigger projects.

⭐ Features

Fungible token minting (ft-mint?)

NFT minting (nft-mint?) with incremental IDs

Read-only counter tracking number of NFTs minted

Deploys without errors (compatible with clarinet check)

📦 Contract Functions
🔎 Read-Only
Function	Description
get-counter	Returns current counter value (number of NFTs minted so far)
✍️ Public Calls
Function	Description
mint-tokens (amount uint)	Mints FT to tx-sender
mint-nft	Mints a new NFT with ID = current counter, increments counter
⚠️ Error Handling

This is a demo contract — no custom error codes are defined. If a mint operation fails, the built-in ft-mint? or nft-mint? will return (err ...).