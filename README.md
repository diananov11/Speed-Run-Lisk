# 🚀 Speed Run Lisk — Deploy & Verify Your First Contracts

This project is part of the **Lisk SEA Campaign Week 1 Challenge**, focused on deploying and verifying smart contracts on **Lisk Sepolia Testnet** using **Scaffold-Lisk**.

---

## 📖 Project Overview

This project demonstrates how to compile, deploy, and verify two smart contracts — an **ERC20 Token (MyToken)** and an **ERC721 NFT (MyNFT)** — on the **Lisk Sepolia testnet**.

✅ **Verified Contracts**

- **MyToken (ERC20):** [0xBc69B1F0Daf36ed116A09f9Bf778CeD1a669eE62](https://sepolia-blockscout.lisk.com/address/0xBc69B1F0Daf36ed116A09f9Bf778CeD1a669eE62#code)
- **MyNFT (ERC721):** [0x61491AFaDabcf22E8e60d47352D8C4c974a36574](https://sepolia-blockscout.lisk.com/address/0x61491AFaDabcf22E8e60d47352D8C4c974a36574#code)

These contracts were deployed and verified using **Hardhat** and **Blockscout** integration.

---

## 🧑‍💻 How to Run Locally

### 1️⃣ Clone the repository

```
git clone https://github.com/diananov11/Speed-Run-Lisk.git
cd Speed-Run-Lisk
```

### 2️⃣ Install dependencies

```
yarn install
```

### 3️⃣ Input your env in folder hardhat

```
cd packages/hardhat
cp .env.example .env // input your private key that contain eth in lisk sepolia testnet
```

### 4️⃣ Deploy contracts in lisk sepolia testnet

```
yarn deploy --network liskSepolia // you must have eth in lisk sepolia testnet
```

### 5️⃣ Verify your contract

```
yarn hardhat-verify --network liskSepolia --contract contracts/MyToken.sol:MyToken <your contract>
yarn hardhat-verify --network liskSepolia --contract contracts/MyNFT.sol:MyNFT <your contract>
```

check on blockscout ` sepolia-blockscout.lisk.com`
<img width="1355" height="511" alt="image_2025-10-30_18-16-21" src="https://github.com/user-attachments/assets/14c5a1de-715c-41c8-9fd4-8eb61fffea2c" />
<img width="1339" height="584" alt="image_2025-10-30_18-17-02" src="https://github.com/user-attachments/assets/eb9fbdde-3c2e-47b9-b019-a88429425620" />


