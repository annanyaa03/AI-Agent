# Monad AI Agent

> Autonomous AI-powered crypto trading agent built on Monad Testnet using MiniMax AI, Pyth Network, and Solidity smart contracts.

---

## Overview

Monad AI Agent is an autonomous on-chain trading system that combines artificial intelligence, live oracle data, and smart contract-based risk management to execute explainable trading decisions.

The system:

* Uses MiniMax AI to analyze market conditions.
* Retrieves live price data from the Pyth Network.
* Applies an EMA-based trading strategy.
* Enforces on-chain safety using the KillSwitch smart contract.
* Executes trades only when predefined risk constraints are satisfied.

---

## Features

* AI-powered trade reasoning
* Explainable decision making
* EMA trading strategy
* Pyth Oracle integration
* KillSwitch smart contract
* Automated trade execution
* Risk management
* Live monitoring dashboard
* Event monitoring
* Monad Testnet deployment

---

## Architecture

```text
                    Dashboard
                        │
                        ▼
                Monad AI Agent
                        │
        ┌───────────────┼───────────────┐
        ▼               ▼               ▼
    MiniMax AI     EMA Strategy    Pyth Oracle
        │                               │
        └───────────────┬───────────────┘
                        ▼
             Trade Decision Engine
                        │
                        ▼
              KillSwitch Contract
                        │
                        ▼
                 Monad Testnet
```

---

## Technology Stack

| Layer           | Technology                |
| --------------- | ------------------------- |
| Frontend        | Next.js (In Progress)     |
| Backend         | Python                    |
| AI              | MiniMax M2.7 (NVIDIA NIM) |
| Oracle          | Pyth Network              |
| Blockchain      | Monad Testnet             |
| Smart Contracts | Solidity                  |
| Framework       | Hardhat                   |

---

## Project Structure

```text
agent/
contracts/
scripts/
test/
docs/
```

---

## Installation

```bash
git clone https://github.com/indrak31/AI-Agent.git

cd AI-Agent

npm install

python -m pip install -r requirements.txt

cp .env.example .env
```

Configure your `.env` file before running the project.

---

## Smart Contract Deployment

```bash
npm run compile

npm test

npm run deploy:hello

npm run deploy:killswitch
```

---

## Running the Project

Dashboard

```bash
python -m agent.dashboard
```

Agent

```bash
python -m agent.agent_loop
```

Utilities

```bash
python -m agent.price_feed

python -m agent.event_listener
```

---

## Safety Mechanisms

The KillSwitch contract provides:

* Daily trading limits
* Maximum trade size
* Cooldown periods
* Emergency stop
* Owner-controlled parameters

---

## AI Workflow

```text
Market Data
      │
      ▼
Pyth Oracle
      │
      ▼
EMA Strategy
      │
      ▼
MiniMax AI
      │
      ▼
Trade Decision
      │
      ▼
KillSwitch Validation
      │
      ▼
Trade Execution
```

---

## Roadmap

* AI reasoning engine
* Monad smart contract deployment
* Web dashboard
* TradingView integration
* Portfolio analytics
* Telegram notifications
* Multi-token support

---

## Team

Built by:

* Indra Kurkute
* Team Members

---

## License

This project is licensed under the MIT License.
