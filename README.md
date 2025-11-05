# End-to-End Encryption Demonstration using PGP (Kleopatra)

## Overview
This project demonstrates how End-to-End Encryption (E2EE) works using **PGP encryption**.  
The goal is to show how a file can be encrypted using a **public key** and decrypted only using the matching **private key**, proving secure communication.

## Tools Used
- **Kleopatra (Gpg4Win Suite)** – for key generation, encryption & decryption
- **Text Editor (Notepad)** – for creating the plaintext message

## Steps Performed

### 1. Generate Key Pair
- Open **Kleopatra**
- `File → New Key Pair → Create OpenPGP Key`
- Enter Name & Email → Create key → Set passphrase

This generates:
- Public Key (used to encrypt)
- Private Key (used to decrypt)

### 2. Create a Plaintext File
Create a file named `secret.txt` and add any confidential message.

Example:

### 3. Encrypt the File
- Right-click `secret.txt`
- Select **Sign and Encrypt**
- Choose **Encrypt Only**
- Select **your own Public Key**
- Output generated: `secret.txt.gpg` (encrypted file)

### 4. Decrypt the File
- Double-click `secret.txt.gpg`
- Enter your key passphrase
- The original `secret.txt` is restored

### 5. Verification (Proof of E2EE)
Try opening `secret.txt.gpg` on a device **without your private key** → Decryption fails.  
This proves the encryption is **end-to-end**.

## Files in Repository
| File | Purpose |
|------|---------|
| `secret.txt` | Original message |
| `secret.txt.gpg` | Encrypted message (ciphertext) |
| `README.md` | Project explanation |

## Conclusion
This demonstration shows how PGP-based encryption forms the foundation of End-to-End Encryption used in:
- Email security (S/MIME, PGP)
- Messaging platforms (Signal, WhatsApp, Telegram)

Only the intended receiver (private key holder) can decrypt the content.

---

### Author
Kirthi Keshav Madival  
CSE Department 


