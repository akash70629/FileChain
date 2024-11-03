# FileChain: Decentralized File Storage System

FileChain is a decentralized file storage system that allows users to securely upload files to a distributed storage network (IPFS) while storing file metadata, like file hash and name, on the blockchain. This setup makes files accessible in a decentralized, secure manner, ensuring a verifiable record of file ownership and metadata on the blockchain.

## Table of Contents

- [Overview](#overview)
- [Tech Stack](#tech-stack)
- [Features](#features)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Future Enhancements](#future-enhancements)
- [License](#license)

---

## Overview

FileChain enables decentralized file storage by combining the InterPlanetary File System (IPFS) and a blockchain for metadata storage. Users can:
- Upload files to IPFS, generating a unique content identifier (CID) for each file.
- Store the CID and other file metadata (e.g., name, timestamp, and uploader address) on the blockchain via a smart contract.
- Retrieve uploaded files securely through their CIDs stored on the blockchain, ensuring data integrity and easy verification.

## Tech Stack

- **Smart Contract Language**: Solidity (for Ethereum or compatible chains like Polygon)
- **Blockchain Platform**: Ethereum (or any EVM-compatible network such as Polygon, Binance Smart Chain, or testnets)
- **Frontend**: HTML, CSS, JavaScript, and optionally, React
- **IPFS**: For decentralized file storage
- **Web3 Library**: Ethers.js or Web3.js for blockchain interaction
- **Wallet**: MetaMask for transaction signing and authentication

---

## Features

- **Decentralized Storage**: Files are stored on IPFS, a peer-to-peer distributed file system.
- **Blockchain Metadata Storage**: File metadata, including file hash, name, and uploader address, is stored on the blockchain.
- **Ownership and Verification**: Each file upload is tied to the uploader’s address, providing verifiable proof of ownership.
- **Data Integrity**: IPFS CIDs ensure that files remain unaltered and can be retrieved with data integrity intact.

---

## Setup and Installation

Follow these steps to set up FileChain on your local machine.

### Prerequisites

1. **Node.js** and **npm** – [Install Node.js](https://nodejs.org/)
2. **MetaMask** – [Install MetaMask](https://metamask.io/) as a browser extension.
3. **Infura Account** – Sign up on [Infura](https://infura.io/) for IPFS access and obtain an API key.

### Installation Steps

1. Clone this repository:

   
bash
   git clone https://github.com/your-username/FileChain.git
   cd FileChain


2. Install dependencies:

   
bash
   npm install


3. Compile and Deploy the Smart Contract:

   - Open the contracts/ folder and locate FileChain.sol.
   - Compile and deploy the smart contract on an EVM-compatible network (e.g., Ethereum testnets like Rinkeby, or Polygon Mumbai).
   - Note down the deployed contract address and ABI for frontend integration.

4. Configure IPFS:

   - Replace YOUR_PROJECT_ID and YOUR_PROJECT_SECRET in src/utils/ipfs.js with your Infura IPFS credentials.

5. Run the Frontend:

   
bash
   npm start


   Open http://localhost:3000 in your browser to start using FileChain.

---

## Usage

1. **Upload a File**:
   - Connect MetaMask to the frontend.
   - Use the file upload form to select a file and upload it to IPFS.
   - Once uploaded, the IPFS CID and file metadata are stored on the blockchain.
  
2. **Retrieve Files**:
   - Files uploaded to FileChain can be retrieved using their CID, accessible from the IPFS network.

3. **Verify Ownership**:
   - The blockchain transaction serves as proof of file upload and ownership tied to the uploader's address.

---

## Future Enhancements

Some ideas for expanding FileChain's capabilities:

1. **Access Control**: Allow users to set access permissions for files.
2. **Enhanced Metadata**: Store additional metadata, such as file description, tags, or file type.
3. **File Search**: Implement search functionality to locate files based on metadata.
4. **Decentralized Identity Integration**: Add DID for enhanced identity verification and access control.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue to help improve FileChain.
--- 
Happy Decentralized Storing with FileChain!
--- 
