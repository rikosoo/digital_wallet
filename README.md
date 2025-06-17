# 💳 Web3 SubWallet – Smart Digital Wallet with Spending Limits

> A decentralized Web3 financial system that allows users to create subcards with personalized spending limits, validating transactions via smart contracts. Perfect for managing expenses of children, employees, or subscriptions.

---

## 📌 Project Overview

**SubWallet** is a **Web3 digital wallet** that provides:

- Registration of tokenized or simulated credit/debit cards  
- Splitting cards into **subcards** with **custom limits**
- **Smart contract validation** of transactions
- Web interface (React) and Mobile App (Flutter)
- High-performance **Go backend**
- Transaction history and spending alerts

---

## 🎯 Pitch

> “Take control of your finances with blockchain security. Create subcards with specific limits for your kids, team, or subscriptions — with automated validation and complete transparency.”

---

## 👥 Target Audience

- Parents managing children's spending
- Entrepreneurs and small business owners
- Web3/crypto-savvy users
- Financial educators
- Fintech companies (potential white-label use)

---

## 📐 Architecture

```
[ Flutter App ]    [ React Web App ] 
       ↓                  ↓
         REST API (Go)
                ↓
+---------------------------+
|           Backend         |  ←→  MongoDB
|           (Go)            |  ←→  Ethereum (Smart Contract in Solidity)
+---------------------------+
```

---

## 🚀 Technologies Used (possible)

| Layer          | Technologies                                            |
|----------------|---------------------------------------------------------|
| Web Frontend   | React.js, Web3Modal, Tailwind CSS                      |
| Mobile App     | Flutter (Dart), web3dart                               |
| Backend        | Go, Gin, MongoDB, JWT, GORM                            |
| Blockchain     | Solidity, Hardhat, Polygon (Mumbai Testnet)           |
| Web3 Integration | Ethers.js / go-ethereum                             |
| Security       | JWT, HTTPS, AES256 encryption, Rate Limiting          |

---

## 📄 Project Scope

### 1. Web3 Authentication
- Login with MetaMask or WalletConnect
- Optional login with email/password

### 2. Card Registration
- Tokenized cards or simulated entries
- Future integration with Open Banking (BACEN)

### 3. Subcard Management
- Create subcards with:
  - Custom name
  - Monthly or per-transaction limits
- Ability to edit or delete

### 4. Solidity Smart Contract
- Validates transactions against subcard limits
- Rejects overspending
- Emits success/failure events on-chain

### 5. Dashboard
- Total and per-card spending
- Transaction history
- Limit alerts

---

## ✅ Functional Requirements

| Code  | Description                             |
|-------|-----------------------------------------|
| FR01  | User must be able to log in via Web3    |
| FR02  | User can register cards and subcards    |
| FR03  | User can define and edit spending limits|
| FR04  | Smart contract must approve or reject transactions |
| FR05  | User can view history and alerts        |

---

## 📜 Business Rules

- Each card can have multiple subcards
- Each subcard has its own spending limit
- Transactions exceeding the limit must be rejected
- Only the wallet owner can manage their cards/subcards
- All transactions are recorded for auditing purposes

---

## 🔍 MVP Scope (Phase 1)

- MetaMask login
- Manual card and subcard creation
- Smart Contract to validate spending
- Web Frontend with spending simulation
- Go Backend + MongoDB

---

## 🧠 Smart Contract Example  (Solidity) - learn


---

## 🧪 Interface Mockup (Structure)

### Home Page
- "Connect Wallet" button
- Display connected wallet address

### Card Management
- List of subcards
- "Add Subcard" button
- Input: name + limit + status

### Transaction Simulator
- Select subcard
- Enter transaction value
- "Simulate Transaction" button
- Response status ✅ or ❌

---

## 📦 Project Structure

```
/backend/         → Go (REST API with Gin)
/contracts/       → Solidity Smart Contracts
/frontend/        → React Web App
/mobile/          → Flutter App
/hardhat/         → Hardhat scripts for testing/deployment
```

---


