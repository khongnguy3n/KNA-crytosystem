# 🔐 KNA Cryptosystem

The KNA cryptosystem, a novel encryption framework based on bitwise inversion, bit position permutation, and noise insertion in binary sequences. Utilizing repeated concatenation and dynamic permutation generated from secret keys, KNA achieves exponential computational complexity for attackers while maintaining linear-time encryption performance. Our analysis demonstrates KNA’s resistance to brute-force and side-channel attacks and its potential to become one of the strongest encryption schemes to date.

---
 
## 📘 Overview

This cryptosystem is designed to:

- Encode binary strings using a repeatable, deterministic algorithm.
- Allow precise decoding with prior knowledge of the transformation steps.
- Provide structure and clarity for further cryptographic experimentation.

---

## ⚙️ Algorithm Steps

### 🔐 **Encryption**

1. **Input** a binary string `B` and an integer `n` (repeat count).
2. **Repeat** `B` `n` times → produce extended string `B'`.
3. **Insert noise bits** (0 or 1) at specific positions: `a, b, c...`.
4. **Invert bits** using a fixed permutation pattern `P`.
5. **Permute positions** using a mapping function `Q`.
6. **Output** the encrypted binary string.

### 🔓 **Decryption**

1. **Input** the encrypted binary string.
2. **Apply inverse permutation** `Q⁻¹` to recover original bit order.
3. **Invert bits back** using pattern `P`.
4. **Remove noise bits** from positions `a, b, c...`.
5. **Split the remaining string** into `n` parts.
6. **Output** the recovered original binary string.

---

## 🖼️ Encryption/Decryption Diagram

![image](https://github.com/user-attachments/assets/f08d048d-ca5e-4572-b0e0-1c538a9f4d5f)

## Document

The full paper is provided in the directory:
https://github.com/khongnguy3n/KNA-crytosystem/blob/main/KNA%20Cryptosystem.pdf


## ✍️ Author

**Khong Nguyen**  
📧 Email: khongnguy3n@gmail.com  
📞 Phone: +49 1624597204  


