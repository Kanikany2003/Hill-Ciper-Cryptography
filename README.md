<h1 align="center">🔒 Hill Cipher Encryption & Decryption 🔓</h1>

<p align="center">
  <strong>A C program that implements the Hill Cipher algorithm to encrypt and decrypt text using matrix-based encryption.</strong>
</p>

---

## 📌 Overview

This project implements **Hill Cipher**, a classical encryption algorithm that uses matrix multiplication for encoding and decoding messages. The encryption process converts plaintext into ciphertext using a key matrix, and decryption recovers the original message using the inverse of the matrix.

- **Encryption:** Converts plaintext into ciphertext using a matrix transformation.
- **Decryption:** Uses the inverse of the key matrix to recover the original text.
- **Supported Matrices:** 2x2 and 3x3 key matrices.

---

## 🚀 Programming Language Used

This project is written in **C**, a low-level and efficient language, making it ideal for implementing cryptographic algorithms.

---

## 🔑 Main Logic

### 🛠 Encryption Process
1. **User provides a key matrix** (2x2 or 3x3) and a plaintext message.
2. The plaintext is converted into numerical values (**A=0, B=1, ..., Z=25**).
3. The message is padded if necessary to fit the matrix size.
4. **Matrix multiplication** is performed between the key matrix and the plaintext blocks.
5. The result is **converted back to letters**, forming the ciphertext.
6. The ciphertext is saved to `ciphertext.txt`.

### 🔓 Decryption Process
1. **User provides the same key matrix** used for encryption.
2. The **inverse of the key matrix** is calculated using modular arithmetic.
3. The ciphertext is converted into numerical values.
4. The **inverse matrix is multiplied** with the ciphertext blocks to recover plaintext.
5. The decrypted message is saved to `plaintext.txt`.
   
<div style="border: 2px solid #ddd; padding: 15px; border-radius: 5px; background: #f8f9fa;">
  <h2> Encryption Example</h2>

  <strong>plaintext.txt</strong>
  <pre style="background:#fff;padding:10px;border-radius:5px;">thisisencryptionhillcipher</pre>

  <strong>Provide the Key Matrix</strong>
  <pre style="background:#fff;padding:10px;border-radius:5px;">2 11<br>3 11</pre>

  <strong>ciphertext.txt</strong>
  <pre style="background:#fff;padding:10px;border-radius:5px;">LEGOGOVZJLFDWPPDYFNYOQDSNR</pre>
</div>

<div style="border: 2px solid #ddd; padding: 15px; border-radius: 5px; background: #f8f9fa;">
  <h2> Decryption Example</h2>

  <strong>ciphertext.txt</strong>
  <pre style="background:#fff;padding:10px;border-radius:5px;">LEGOGOVZJLFDWPPDYFNYOQDSNR</pre>

  <strong>Provide the Key Matrix</strong>
  <pre style="background:#fff;padding:10px;border-radius:5px;">2 11<br>3 11</pre>

  <strong>plaintext.txt</strong>
  <pre style="background:#fff;padding:10px;border-radius:5px;">thisisencryptionhillcipher</pre>
</div>

