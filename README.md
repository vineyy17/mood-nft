# MoodNft Project

MoodNft is a dynamic NFT project that reflects the owner's mood. Each NFT can be in either a happy or sad state, with the ability to flip between these moods.

## Features

- Mint NFTs with an initial happy mood
- Flip the mood of owned NFTs
- Dynamic metadata that changes based on the NFT's current mood
- Fully on-chain SVG images

## Technologies

- Solidity 0.8.20
- Foundry/Forge for development and testing
- OpenZeppelin for ERC721 implementation

## Setup

1. Clone the repository
2. Install dependencies:
   ```bash
   make install
   ```

## Building

To build the project, run:

```bash
make build
```

## Testing

Run tests with:

```bash
make test
```

For zkSync specific tests:

```bash
make zktest
```

## Deployment

To deploy the contract:

```bash
make deploy
```

For network-specific deployment (e.g., Sepolia), use:

```bash
make deploy ARGS="--network sepolia"
```

## Interacting with the Contract

- To mint a new NFT:
  ```bash
  make mint
  ```

- To flip the mood of an NFT:
  ```bash
  make flip
  ```

## Development Commands

- Format code: `make format`
- Update dependencies: `make update`
- Run local Anvil chain: `make anvil`

## Environment Setup

Create a `.env` file in the root directory with the following variables:

```
SEPOLIA_RPC_URL=your_sepolia_rpc_url
ETHERSCAN_API_KEY=your_etherscan_api_key
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.
