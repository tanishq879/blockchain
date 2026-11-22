# blockchain
# Blockchain Voting DApp

A blockchain-based decentralized voting application developed using **Solidity, Remix IDE, MetaMask, Sepolia Testnet, HTML, CSS, JavaScript, and Ethers.js**.

The project demonstrates how blockchain technology can be used to build a transparent voting system where each wallet address is allowed to vote only once.

# 1. Voting System

## Overview

The Voting System is a decentralized application (DApp) that allows users to vote for predefined candidates using their MetaMask wallet.

The smart contract records votes on the blockchain and prevents users from voting more than once.

## Features

- Three predefined candidates:
  - Candidate A
  - Candidate B
  - Candidate C
- MetaMask wallet connection.
- One vote per wallet address.
- Prevention of duplicate voting.
- Candidate validation.
- Automatic vote count updates.
- Displays candidate voting results.
- Blockchain transaction confirmation.
- Displays transaction and error status.

## Technologies Used

- Solidity
- Remix IDE
- MetaMask
- Ethereum Sepolia Testnet
- HTML
- CSS
- JavaScript
- Ethers.js

## Smart Contract Functions

| Function | Description |
|---|---|
| `getCandidates()` | Returns the list of candidates. |
| `candidates(index)` | Retrieves a candidate using its index. |
| `getVotes(candidate)` | Returns the vote count for a candidate. |
| `hasVoted(address)` | Checks whether an address has already voted. |
| `vote(candidate)` | Casts a vote for a candidate. |
| `owner()` | Returns the contract owner's address. |

## How the Voting System Works

1. The Voting smart contract is deployed on the Sepolia Testnet.
2. Candidates are initialized through the constructor.
3. The user opens the voting application.
4. The user connects their MetaMask wallet.
5. The application checks the connected blockchain network.
6. The user selects a candidate.
7. The smart contract checks whether the wallet has already voted.
8. If eligible, the vote is recorded on the blockchain.
9. The updated voting results are displayed.

## Deployment and Execution

1. Open [Remix IDE](https://remix.ethereum.org/).
2. Create a Solidity file named `Voting.sol`.
3. Write the Voting smart contract.
4. Compile the contract using a compatible Solidity compiler.
5. Connect MetaMask to the Sepolia Testnet.
6. Select the Voting contract in Remix.
7. Enter the candidate names in the constructor, for example:

```text
["A","B","C"]
```

8. Select Injected Provider - MetaMask.
9. Deploy the contract.
10. Confirm the deployment transaction in MetaMask.
11. Copy the deployed contract address.
12. Add the contract address and ABI to the frontend JavaScript file.
13. Open the frontend using a local development server.
14. Connect MetaMask and interact with the voting application.

## Testing

The following test cases are included in the project:

- Successful voting using a wallet account.
- Prevention of duplicate voting from the same account.
- Voting using a second wallet account.
- Rejection of invalid candidate names.
- Verification of candidate vote counts.

Example test results should be added after executing the test cases.

| Candidate | Votes |
|---|---:|
| Candidate A | To be updated |
| Candidate B | To be updated |
| Candidate C | To be updated |

# 2. Frontend Application

## Overview

The frontend provides a user-friendly interface to interact with the Voting smart contract.

## Frontend Features

- Connect MetaMask wallet.
- Display connected wallet address.
- Display current blockchain network.
- Show available candidates.
- Display total votes for each candidate.
- Allow eligible users to vote.
- Disable voting after a successful vote.
- Refresh voting results.
- Display transaction and error messages.

# 3. Development Environment

## What is Solidity?

Solidity is a programming language used to create smart contracts for Ethereum-compatible blockchains.

## What is Remix IDE?

Remix is an online development environment used to write, compile, deploy, and interact with Solidity smart contracts.

## What is MetaMask?

MetaMask is a cryptocurrency wallet that connects the frontend application to blockchain networks and allows users to approve transactions.

## What is Sepolia Testnet?

Sepolia is an Ethereum test network used to deploy and test smart contracts without spending real ETH.

## What is Ethers.js?

Ethers.js is a JavaScript library used to connect the frontend application with Ethereum-compatible blockchain networks and smart contracts.

# 4. Project Structure

```text
Voting-DApp/
│
├── index.html
├── style.css
├── script.js
├── Voting.sol
└── README.md
```

# 5. Learning Outcomes

Through this project, I learned:

- Basics of blockchain technology.
- Solidity smart contract development.
- Smart contract compilation and deployment.
- MetaMask wallet integration.
- Interaction with Ethereum Sepolia Testnet.
- Frontend and smart contract integration.
- Using Ethers.js to interact with contracts.
- Understanding blockchain transactions.
- Implementing duplicate voting prevention.
- Validating candidate names.
- Retrieving blockchain data.
- Testing smart contract functions.

---

**Project:** Decentralized Voting DApp  
**Network:** Ethereum Sepolia Testnet  
**Development Tools:** Remix IDE, MetaMask and VS Code
