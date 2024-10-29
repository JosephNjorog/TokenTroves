# TokenTroves

TokenTroves is a decentralized platform that gamifies task management by leveraging blockchain technology. Users can earn NFTs and climb the leaderboard by completing tasks. The platform also integrates a Telegram bot for seamless notifications and interactions.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Architecture](#architecture)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Directory Structure](#directory-structure)
- [Backend Setup](#backend-setup)
  - [Environment Variables](#environment-variables)
  - [Running the Backend](#running-the-backend)
- [Frontend Setup](#frontend-setup)
  - [Running the Frontend](#running-the-frontend)
- [Smart Contracts Setup](#smart-contracts-setup)
  - [Deploying Smart Contracts](#deploying-smart-contracts)
- [Telegram Bot Setup](#telegram-bot-setup)
  - [Running the Telegram Bot](#running-the-telegram-bot)
- [Testing](#testing)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

TokenTroves is designed to enhance productivity by turning task management into an engaging experience. Users can:

- Create and manage tasks.
- Earn NFTs as rewards for completing tasks.
- View their progress and compete on the leaderboard.
- Receive notifications and interact with the platform via a Telegram bot.

## Features

- **Task Management**: Users can create, update, and delete tasks.
- **NFT Rewards**: Users earn NFTs for completing tasks.
- **Leaderboard**: Users compete on a leaderboard based on task completion.
- **Community Feed**: Users can share their progress and engage with the community.
- **Notifications**: Users receive notifications about task updates and NFT rewards.
- **Telegram Bot**: Users can interact with the platform via a Telegram bot.

## Architecture

The project consists of the following components:

- **Backend**: Node.js with Express and MongoDB for API and database.
- **Frontend**: React for the user interface.
- **Smart Contracts**: Solidity for NFT and task management on the Ethereum blockchain.
- **Telegram Bot**: Node.js bot for Telegram interactions.

## Technologies Used

- **Backend**: Node.js, Express, MongoDB, Mongoose
- **Frontend**: React, Context API, Hooks
- **Smart Contracts**: Solidity, Truffle
- **Telegram Bot**: Node.js, Telegraf
- **Others**: JWT, Bcrypt, Jest/Mocha, CSS

## Getting Started

### Prerequisites

Make sure you have the following installed:

- Node.js
- npm
- MongoDB
- Truffle
- Ganache (optional, for local Ethereum blockchain)
- Telegram account (for bot setup)

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/TokenTroves.git
   cd TokenTroves
   ```

2. Install dependencies:
   ```sh
   npm install
   ```

## Directory Structure

```plaintext
TokenTroves/
  ├── backend/
  │   ├── controllers/
  │   ├── models/
  │   ├── routes/
  │   ├── services/
  │   ├── utils/
  │   ├── app.js
  │   ├── server.js
  │   └── config/
  ├── frontend/
  │   ├── public/
  │   ├── src/
  │   │   ├── components/
  │   │   ├── contexts/
  │   │   ├── hooks/
  │   │   ├── services/
  │   │   ├── App.js
  │   │   ├── index.js
  │   │   └── styles/
  ├── smart_contracts/
  │   ├── contracts/
  │   ├── migrations/
  │   ├── test/
  │   └── truffle-config.js
  ├── telegram_bot/
  │   ├── bot.js
  │   ├── config.js
  │   └── utils/
  ├── test/
  │   ├── backend/
  │   └── frontend/
  ├── package.json
  ├── README.md
  └── .gitignore
```

## Backend Setup

### Environment Variables

Create a `.env` file in the `backend` directory with the following variables:

```plaintext
MONGO_URI=<your_mongodb_uri>
JWT_SECRET=<your_jwt_secret>
```

### Running the Backend

1. Navigate to the `backend` directory:
   ```sh
   cd backend
   ```

2. Start the server:
   ```sh
   npm start
   ```

The backend server will run on `http://localhost:5000`.

## Frontend Setup

### Running the Frontend

1. Navigate to the `frontend` directory:
   ```sh
   cd frontend
   ```

2. Start the React app:
   ```sh
   npm start
   ```

The frontend will run on `http://localhost:3000`.

## Smart Contracts Setup

### Deploying Smart Contracts

1. Navigate to the `smart_contracts` directory:
   ```sh
   cd smart_contracts
   ```

2. Install Truffle dependencies:
   ```sh
   npm install
   ```

3. Compile the contracts:
   ```sh
   truffle compile
   ```

4. Deploy the contracts to the local blockchain (Ganache):
   ```sh
   truffle migrate
   ```

## Telegram Bot Setup

### Running the Telegram Bot

1. Navigate to the `telegram_bot` directory:
   ```sh
   cd telegram_bot
   ```

2. Create a `config.js` file with your Telegram bot token:
   ```plaintext
   module.exports = {
     TOKEN: '<your_telegram_bot_token>',
   };
   ```

3. Start the bot:
   ```sh
   node bot.js
   ```

## Testing

1. Navigate to the `test` directory:
   ```sh
   cd test
   ```

2. Run tests:
   ```sh
   npm test
   ```

Tests are written using Jest/Mocha for both frontend and backend.

## Deployment

### Backend Deployment

1. Deploy the backend to Heroku, DigitalOcean, or any other cloud provider.
2. Set environment variables for the production environment.

### Frontend Deployment

1. Deploy the frontend to Vercel, Netlify, or any other static site hosting provider.
2. Ensure the API endpoints are correctly set for the production environment.

### Smart Contracts Deployment

1. Deploy the smart contracts to Ethereum mainnet or any other testnet using Truffle.
2. Update the contract addresses in the backend and frontend configurations.

### Telegram Bot Deployment

1. Deploy the Telegram bot to a server (e.g., AWS EC2, DigitalOcean Droplet).
2. Ensure the bot is running and accessible.

## Contributing

We welcome contributions to TokenTroves! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch for your feature or bug fix:
   ```sh
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```sh
   git commit -m 'Add some feature'
   ```
4. Push to the branch:
   ```sh
   git push origin feature-name
   ```
5. Open a Pull Request.

Please ensure your code follows our coding standards and includes tests for new functionality.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

This comprehensive README should provide a clear understanding of the project structure, setup instructions, and overall functionality of TokenTroves. If you have any further questions or need additional details, feel free to ask!
