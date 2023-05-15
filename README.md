# FEST TOKEN APP

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Challenges](#challenges)
- [Getting Started](#getting-started)
- [Demo](#demo)
- [Technologies Used](#technologies-used)
- [Contributors](#contributors)

## Introduction
FEST TOKEN APP is a web application designed to address the issue of students' unrecognized contributions to extracurricular activities. With this decentralized digital currency system, college administrators and event coordinators can easily reward students with digital currency for their hard work and dedication.

## Features
- Administrators can add a token amount to a specific user to acknowledge their contributions
- For every user, a wallet is created containing the private and public keys
- Students can transfer tokens among each other with some taxes (if transfer occurs between different batches)
- Tokens are auto-expired when a student graduates

## Challenges
- Difficulty in implementing burn token function on Openzeppelin, but finally we came with an idea to modify the ERC20 token contract by overriding the _burn function
- Issues while deploying the website on GitHub. So, we merged it into a single page. But, on the localhost, it's working completely fine and is also shown in the video.
- Issues with adding taxes when a student tries to do a transfer token. We have finally removed that error by assigning a batch flag to each student.

## Getting Started
To get started with FEST TOKEN APP, you can clone this repository and run the web application locally.
1. Write your smart contract in backend folder
2. Start the hardhat node with npx hardhat node
3. Deploy the contract on local hardhat node => npx hardhat run src/backend/scripts/deploy.js --network localhost
4. Start the npm server for frontend to react => npm run start


## Demo
Check out the [demo video](https://youtu.be/AssSGAcXJAU) to see FEST TOKEN APP in action.

## Technologies Used
- Solidity
- Web3.js
- React.js
- Node.js
- Hardhat
- Polygon

## Contributors
- [Divyam Patel](https://github.com/pateldivyam26)
- [Pratham Chaurasia](https://github.com/PrathamGit-dev)
