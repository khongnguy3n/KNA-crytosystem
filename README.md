# 🔐 KNA Cryptosystem

The **KNA Cryptosystem** is a custom-designed lightweight encryption algorithm that utilizes **bitwise inversion**, **bit permutation**, and **noise injection** for secure data encoding. It is structured to be simple, fast, and resistant to basic attacks.

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

![image](https://github.com/user-attachments/assets/ddc4a8c6-4b72-4507-a3e2-dd75f545c8b3)


## 📁 File Structure


---

## ✍️ Author

**Khong Nguyen**  
📧 Email: khongnguy3n@gmail.com  
📞 Phone: +49 1624597204  

---

## 🌐 License

This project is released under the MIT License.
