## 🔐 Digital Signature Verification Using MetaMask & Blockchain

A blockchain-based digital signature verification system built using React, Ethereum cryptography, and the MetaMask cryptocurrency wallet.
This project demonstrates how secure message signing and verification can be achieved using public-key cryptography (ECDSA) without exposing private keys or relying on centralized authorities.

This project was developed as part of a **Final Year Engineering Project** and is suitable for academic submission, portfolio showcase, and Web3 learning.

---

## 📌 Problem Statement
Traditional digital signature verification systems are often:
- Centralized and opaque
- Dependent on trusted third parties
- Costly for end users
- Vulnerable to forgery and identity fraud
With the exponential growth of digital transactions, forged signatures and identity fraud have become major security concerns in legal, financial, and governmental systems.

> ### _**In 2020, _India recorded a 141% increase in identity fraud, resulting in losses of nearly ₹1.85 trillion, highlighting the urgent need for stronger and verifiable_**_

This project addresses these issues by implementing blockchain-based digital signature verification using MetaMask, enabling free, transparent, and tamper-resistant validation.


## 🎯 Objectives
- To implement digital signature generation and verification
- To demonstrate authentication, integrity, and non-repudiation
- To eliminate dependency on paid, off-chain verification services
- To securely verify signatures using Ethereum public keys
- To provide a clean and user-friendly UI for signing and verification

---

## 🧩 Methodology
The digital signature process consists of two main phases:

🔹 1. Signing Phase
- User enters a message
- Message is hashed using a cryptographic hash function
- Hash is signed using the private key stored securely in MetaMask
- A digital signature is generated and returned to the application

🔹 2. Verification Phase
- Signature and original message are provided
- Public key (Ethereum address) is recovered from the signature
- Message hash is recomputed
- Signature validity is verified by comparing hashes
- This ensures message authenticity and integrity.
---
## 🔐 Cryptography & Security Design
- Signature Algorithm: ECDSA (Elliptic Curve Digital Signature Algorithm)
- Elliptic Curve: secp256k1 (Ethereum standard)
- Hashing: Cryptographic hash for fixed-length message digest
- Key Management:
  - Private keys never leave MetaMask
  - Only public keys are used for verification

## 🔒 Security Guarantees
- Authentication of the signer
- Integrity of the message
- Non-repudiation
- Resistance to forgery and tampering

---


## 🖥️ Application Preview

### 🔹 Message Signing
![Sign Message](Screenshots/sign-message.png)

### 🔹 Signature Verification
![Verify Signature](Screenshots/verify-message.png)

---

## 🧠 How It Works

1. User enters a message
2. MetaMask prompts the user to **sign the message**
3. A cryptographic signature is generated using **ECDSA**
4. The app recovers the signer’s **Ethereum address**
5. The recovered address is compared with the claimed signer
6. Verification result is displayed instantly

---

## 🔐 Cryptography Behind the Scenes

- **Elliptic Curve Digital Signature Algorithm (ECDSA)**
- Curve used: **secp256k1** (Ethereum standard)
- Message signing via `personal_sign`
- Address recovery using `ethers.js`

> 🛑 Private keys never leave MetaMask.  
> This application only works with **public cryptographic data**.

---

## 🛠️ Tech Stack

| Technology | Usage |
|----------|------|
| React (CRA) | Frontend framework |
| Ethers.js | Ethereum interaction & signature recovery |
| MetaMask | Wallet & message signing |
| JavaScript (ES6) | Core logic |
| HTML / CSS | UI styling |

---

## 🚀 Getting Started (Local Setup)

### 1️⃣ Clone the repository
```bash
git clone https://github.com/chetanmeshram10/Digital-Signature-Verification-Using-MetaMask-Cryptocurrency-Wallet.git
cd Digital-signature-verification
```

2️⃣ Install dependencies
```
npm install --legacy-peer-deps
```

3️⃣ Start the development server
```
npm start
```

Open in browser:
```
http://localhost:3000
```

## 🦊 MetaMask Requirements
  - Install MetaMask browser extension
  - Use Chrome / Brave / Edge
  - Any Ethereum network works (no gas required for signing)

---

## 📂 Project Structure
```
src/
 ├── App.js
 ├── SignMessage.js
 ├── VerifyMessage.js
 ├── SuccessMessage.js
 ├── ErrorMessage.js
 └── index.js

public/
 └── index.html
```
---


## 👨‍💻 Author

## **Chetan Meshram**

**Mtech IT IIITA Student | Blockchain & Cryptography Enthusiast**

🔗 GitHub: https://github.com/chetanmeshram10

---

## ⭐ Support
If you found this project useful:
- ⭐ Star the repository
- 🍴 Fork it
- 📢 Share
