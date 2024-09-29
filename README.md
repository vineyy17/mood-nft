# MoodNft

MoodNft is a dynamic, on-chain NFT smart contract built with Solidity. It allows owners to mint NFTs with two possible moods: Happy or Sad. The NFT's mood can be flipped by the owner, and the NFT's metadata, including attributes, reflects the current mood.

## Features

- **ERC-721 compliant**: Follows the ERC-721 standard for NFTs.
- **Dynamic metadata**: NFT mood can change between "Happy" and "Sad," and this is reflected in the token metadata.
- **On-chain SVG images**: NFT metadata is stored fully on-chain, including mood-dependent SVG image URIs.

## Contract Overview

- `mintNft()`: Mint a new NFT with the default "Happy" mood.
- `flipMood(uint256 tokenId)`: Flip the mood of an NFT between "Happy" and "Sad." Only the owner of the NFT can perform this action.
- `tokenURI(uint256 tokenId)`: Returns the on-chain JSON metadata, including the image and mood-based attributes.

## Mood-Based Metadata

- **Happy Mood**:
  - Image: Displays a happy SVG image.
  - Attribute: `"cheerfulness": 100`
  
- **Sad Mood**:
  - Image: Displays a sad SVG image.
  - Attribute: `"moodiness": 100`

## Prerequisites

- [Solidity ^0.8.0](https://docs.soliditylang.org/en/latest/)
- [OpenZeppelin Contracts](https://docs.openzeppelin.com/contracts/4.x/)
