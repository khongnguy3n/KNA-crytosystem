readme_content = """
# 🔐 KNA Cryptosystem

**A novel symmetric encryption system based on bit inversion, position permutation, iterative chaining, and noise injection.**

## 📌 Overview

The KNA cryptosystem is a new approach to symmetric encryption designed for conceptual clarity and computational simplicity. It introduces a structural method using:

- **Bit Inversion**  
- **Bit Position Permutation**  
- **Iterative Chaining**  
- **Noise Injection**

It is primarily intended for theoretical exploration, research, and lightweight secure encoding.

---

## 🧠 Key Components

1. **Bit Inversion**  
   Each bit is flipped according to a deterministic or key-dependent rule.

2. **Position Permutation**  
   Bit positions are shuffled using a secret permutation key.

3. **Chaining**  
   The output is re-fed into the algorithm for multiple rounds.

4. **Noise Injection**  
   Extra bits are added to obscure the structure and increase complexity.

---

## 📊 Encryption / Decryption Table (Example)

Below is a simplified example of one encryption and decryption cycle with an 8-bit binary message:

| Step                     | Binary Data     | Description                           |
|--------------------------|-----------------|---------------------------------------|
| **Original Plaintext**   | `10110010`      | Input message                         |
| **Bit Inversion**        | `01001101`      | Flip each bit                         |
| **Permutation**          | `10010110`      | Rearranged using permutation key      |
| **Noise Injection**      | `110010111011`  | Noise bits added                      |
| **Ciphertext (output)**  | `110010111011`  | Final encrypted message               |

To **decrypt**, reverse each step in the correct order:

| Step                     | Binary Data     | Description                           |
|--------------------------|-----------------|---------------------------------------|
| **Ciphertext (input)**   | `110010111011`  | Encrypted message                     |
| **Noise Removal**        | `10010110`      | Extract only true data bits           |
| **Reverse Permutation**  | `01001101`      | Undo bit position shuffling           |
| **Bit Re-Inversion**     | `10110010`      | Flip bits again                       |
| **Recovered Plaintext**  | `10110010`      | Original input restored               |

---

## ⚙️ Applications

- Educational cryptography
- Theoretical modeling of symmetric ciphers
- Custom lightweight encryption schemes

---

## 📁 Project Contents

- `KNA_Specification.pdf`: Technical paper with algorithm and theory
- `example_code/`: Source code in Python
- `examples/`: Input/output demonstrations

---

## 📜 License

This project is open for collaborative academic research and educational use. Proper attribution is appreciated.

---

## 🙋‍♂️ Author

**Nguyen Minh Chinh**  
Email: [Khongnguy3n@gmail.com](mailto:Khongnguy3n@gmail.com)  
Phone: +49 162 459 7204
"""

# Write to README.md file
with open("README.md", "w", encoding="utf-8") as f:
    f.write(readme_content)

print("README.md created successfully.")
