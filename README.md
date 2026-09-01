# NFT Marketplace

This project is a full-stack decentralized application (dApp) that enables users to create, list, and trade NFTs on a blockchain. It demonstrates proficiency in smart contract development and integration with modern web technologies.

## Features

- Create and mint new NFTs.
- List NFTs for sale on the marketplace.
- Trade (buy/sell) NFTs securely on the blockchain.
- View a dashboard of created NFTs.
- View a dashboard of owned NFTs.

## Tech Stack

[![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)](https://nextjs.org/) [![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://reactjs.org/) [![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/) [![Hardhat](https://img.shields.io/badge/Hardhat-20232A?style=for-the-badge&logo=hardhat&logoColor=white)](https://hardhat.org/) [![Solidity](https://img.shields.io/badge/Solidity-363636?style=for-the-badge&logo=solidity&logoColor=white)](https://docs.soliditylang.org/) [![Ethers.js](https://img.shields.io/badge/Ethers.js-2A2E35?style=for-the-badge&logo=ethereum&logoColor=white)](https://docs.ethers.io/v5/) [![IPFS](https://img.shields.io/badge/IPFS-65C0D4?style=for-the-badge&logo=ipfs&logoColor=white)](https://ipfs.io/) [![Web3Modal](https://img.shields.io/badge/Web3Modal-000000?style=for-the-badge&logo=web3.js&logoColor=white)](https://github.com/Web3Modal/web3modal) [![Axios](https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white)](https://axios-http.com/)

## Setup

1.  **Clone the repository:**
    ```bash
    git clone [repository-url]
    cd nft-market
    ```
2.  **Install dependencies:**
    ```bash
    npm install
    ```
3.  **Configure Hardhat and deploy smart contracts:**
    *   Refer to `hardhat.config.js` for network configurations.
    *   Compile smart contracts:
        ```bash
        npx hardhat compile
        ```
    *   Deploy smart contracts to your chosen network (e.g., local development network):
        ```bash
        npx hardhat run scripts/deploy.js --network localhost
        ```
4.  **Update `config.js` with deployed contract addresses.**
5.  **Start the Next.js development server:**
    ```bash
    npm run dev
    ```
    The application will be accessible at `http://localhost:3000`.

## Usage

1.  Connect your Web3 wallet (e.g., MetaMask) to the dApp.
2.  Navigate to the "Create NFT" page to mint a new NFT.
3.  List your newly created NFT for sale on the marketplace.
4.  Browse existing NFTs and purchase them.
5.  View your created and owned NFTs on the respective dashboard pages.

## Project Structure

.|
├── components/
├── pages/
│   ├── _app.js
│   ├── create-item.js
│   ├── creator-dashboard.js
│   ├── index.js
│   └── my-assets.js
├── contracts/
│   ├── NFT.sol
│   └── NFTMarket.sol
├── public/
│   ├── manifest.json
│   └── robots.txt
├── styles/
│   └── main.css
├── .gitattributes
├── config.js
├── hardhat.config.js
├── next.config.js
├── package-lock.json
├── package.json
├── postcss.config.js
└── tailwind.config.js

## Interview Questions

1.  Explain the role of `NFT.sol` and `NFTMarket.sol` in the overall architecture of this NFT marketplace. How do they interact to facilitate NFT creation and trading?
2.  How does IPFS contribute to the decentralized nature of this NFT marketplace? Describe the flow of data when a user creates a new NFT, specifically focusing on how the NFT's metadata and media are handled.
3.  This project uses Next.js, React, and Tailwind CSS for the frontend, and Hardhat, Solidity, Ethers.js, Web3Modal, and Axios for the backend/blockchain interaction. Discuss the key advantages of using this combination of technologies for building a dApp, particularly regarding development efficiency, user experience, and blockchain integration.
