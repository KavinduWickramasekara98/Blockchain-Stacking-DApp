
# Blockchain Staking Decentralization Web Application

## Overview

This project is a blockchain-based staking smart contract developed in Solidity. The contract allows users to stake tokens and earn rewards over time. The front-end interface is developed using Next.js, React, and Tailwind CSS, providing a seamless user experience for interacting with the smart contract. Users can connect their MetaMask wallet, stake tokens, view their wallet balance, and claim rewards directly from the interface.

<details><summary>Image start</summary>
   <img src="https://github.com/user-attachments/assets/ed40086a-f74b-4cdb-a0f9-be6d887487ba" width=35% height=35%>
</details>
<details><summary>After Connect Wallet </summary>
   <img src="https://github.com/user-attachments/assets/c3a37754-d981-4677-8f2b-154e1a7f82e2" width=35% height=35%>
</details>
<details><summary>stacking 100 RT Tokens</summary>
   <img src="https://github.com/user-attachments/assets/47f1d115-f004-46e4-949c-53c88146c878" width=35% height=35%>
</details>


## Features

Staking: Users can stake their tokens into the contract and start earning rewards based on the amount staked and the duration of the stake.
Rewards: Users accumulate rewards over time, which they can claim at any point.
Withdrawal: Users can withdraw their staked tokens from the contract at any time.
MetaMask Integration: The application is integrated with MetaMask, allowing users to connect their wallet and interact with the smart contract.
Real-Time Data: The UI displays the user's wallet balance, staked amount, and accumulated rewards in real-time.
Infura API: The project uses the Infura API to connect to the Ethereum blockchain, ensuring reliable and scalable access to the network.
Smart Contract Details
The smart contract is written in Solidity and implements the following features:

Staking and Rewards Calculation: The contract calculates rewards based on the time the tokens have been staked and the predefined reward rate.
Security Features: The contract uses ReentrancyGuard to prevent reentrancy attacks and includes custom errors to handle failed transactions and invalid inputs.
Token Transfers: The contract interacts with ERC-20 tokens to handle staking, rewards, and withdrawals.
## Key Functions
stake(uint256 amount): Allows users to stake a specified amount of tokens.
withdraw(uint256 amount): Allows users to withdraw their staked tokens.
claimReward(): Allows users to claim their accumulated rewards.
rewardPerToken(): Calculates the reward per token based on the staking duration and total supply.
earned(address account): Returns the total rewards earned by a specific user.

## Front-End (UI) Development
The front-end of the application is built using modern web technologies:

Next.js: Provides the foundation for the React-based web application, enabling server-side rendering and optimized performance.
React: Used for building the dynamic and interactive user interface components.
Tailwind CSS: A utility-first CSS framework that is used for styling the application, making it responsive and visually appealing.
MetaMask: Integrated to allow users to connect their Ethereum wallets and interact with the blockchain directly from their browser.
Infura API: Used to interact with the Ethereum blockchain, ensuring seamless connectivity and transactions.
Setup Instructions
Prerequisites
Node.js and npm installed
MetaMask extension installed in your browser
Infura account with a project ID
Smart Contract Deployment
Install dependencies:

bash
Copy code
npm install
Compile and deploy the smart contract to the Ethereum network using Truffle or Hardhat.

Update the contract address and ABI in your front-end application.

## Front-End Setup
Clone the repository:

bash
Copy code
git clone https://github.com/KavinduWickramasekara98/Blockchain-Stacking-DApp.git
cd staking-dapp
Install front-end dependencies:

bash
Copy code
npm install
Configure the Infura API in your project by adding your project ID to the environment variables.

## Start the development server:

bash
Copy code
npm run dev
Open your browser and navigate to http://localhost:3000 to interact with the staking application.

## Usage
Connect MetaMask: Click on the "Connect Wallet" button to connect your MetaMask wallet to the application.
Stake Tokens: Enter the amount of tokens you wish to stake and click "Stake."
View Rewards: Monitor your accumulated rewards in real-time on the dashboard.
Claim Rewards: Click "Claim Rewards" to withdraw your rewards to your wallet.
Withdraw Staked Tokens: If you wish to withdraw your staked tokens, enter the amount and click "Withdraw."
Future Enhancements
Multi-Token Support: Add support for staking multiple types of tokens.
Advanced Analytics: Provide users with more detailed insights and analytics about their staking activities.
Mobile Support: Improve the responsiveness and usability of the application on mobile devices.
License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments
OpenZeppelin: For providing secure and reusable smart contract libraries.
Infura: For their reliable Ethereum API services.
MetaMask: For enabling seamless Ethereum wallet integration.
