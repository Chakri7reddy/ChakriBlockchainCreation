
# 🚀 Build a Simple Blockchain Simulation

## 📖 Overview

This project is a simple blockchain simulation built using **Node.js**, designed to demonstrate understanding of core blockchain concepts like block linking, hashing, validation, and optional proof-of-work.To view in real UI-based interaction check this https://blockchain-frontend-eosin.vercel.app/

The project fulfills the requirements of the assignment by implementing:

- ✅ Block structure (index, timestamp, transactions, hashes)
- ✅ Hashing with SHA-256
- ✅ Blockchain class to manage chain and validate integrity
- ✅ Tampering detection mechanism
- ✅ Optional: Basic Proof-of-Work (Bonus)
- ✅ Optional: Ability to dynamically add transactions before mining (Bonus)

## 🎯 Objective

> Simulate the core features of a blockchain to understand how block data, cryptographic hashes, and validation work together to ensure blockchain integrity.

## 🛠️ Tech Stack

- **Language:** JavaScript (Node.js)
- **Hashing Algorithm:** SHA-256 (via `crypto` module)

## 📂 Project Structure

```
SimpleBlockchain/
├── node_modules/             # Dependencies
├── src/
│   ├── blockchain.js         # Blockchain & Block classes
│   ├── keygenerator.js       # Generates keys (optional)
│   └── main.js               # Entry point — builds & tests the blockchain
├── package.json              # Project configuration & scripts
├── package-lock.json         # Dependency lock file
└── README.md                 # Project documentation
```

## ⚙️ Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/Chakri7reddy/ChakriBlockchainCreation.git
   cd ChakriBlockchainCreation/SimpleBlockchain
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Run the simulation**
   ```bash
   node src/main.js
   ```

## 🧩 Features

### ✅ Block Structure
Each block contains:
- **Index** — Block number in the chain.
- **Timestamp** — When the block was created.
- **Transactions** — Dummy transactions (with optional dynamic addition).
- **Previous Hash** — Link to the previous block's hash.
- **Current Hash** — SHA-256 hash of current block data.
- **Nonce** — Used for proof-of-work.

### ✅ Hashing
- Uses SHA-256 to hash the block’s contents securely.
- Hash includes block data and previous block’s hash for integrity.

### ✅ Blockchain Class
- Manages the chain of blocks.
- Methods to:
  - Add new blocks.
  - Validate chain integrity (detect tampering).
  - (Optional) Perform Proof-of-Work.

### 💡 Proof-of-Work (Optional Bonus)
- Adds computational effort to block creation.
- Adjustable difficulty (currently: hash must start with leading zeros).

### 🔍 Tampering Detection
- Includes a demonstration of tampering with block data.
- Validation method will detect inconsistencies and flag the chain as invalid.

## 🖥️ Output Example

```bash
Adding a new block...
Mining block...
Block successfully mined!

Blockchain valid? true

Tampering with the blockchain...
Blockchain valid? false
```

## 📚 Concepts Demonstrated

- Blockchain fundamentals
- Cryptographic hash functions
- Proof-of-Work (PoW)
- Chain validation and tamper detection
- Transactions management

## 🧩 Future Enhancements (Optional)
- Add multiple wallets & transaction signatures
- Build REST API to interact with the blockchain
- Create a web interface for easier interaction
- Persist blockchain data in storage

## 🤝 Contribution

Pull requests are welcome. Fork the repo and make your improvements!

## 📄 License

This project is open-source under the [MIT License](LICENSE).


---

## 🌟 If you find this project helpful, feel free to star it!

---
