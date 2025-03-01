# Hill-Ciper-Cryptography
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hill Cipher Encryption & Decryption</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            background-color: #f4f4f4;
            color: #333;
            padding: 20px;
        }
        h1, h2 {
            color: #0056b3;
        }
        .container {
            max-width: 800px;
            margin: auto;
            background: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
        code {
            background: #f4f4f4;
            padding: 2px 5px;
            border-radius: 5px;
            font-weight: bold;
            color: #d63384;
        }
        pre {
            background: #eee;
            padding: 10px;
            border-radius: 5px;
            overflow-x: auto;
        }
        .footer {
            margin-top: 20px;
            font-size: 14px;
            text-align: center;
            color: #666;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>🔐 Hill Cipher Encryption & Decryption</h1>
        <p>This project implements the <strong>Hill Cipher</strong>, a classic cryptographic algorithm that encrypts and decrypts messages using matrix multiplication.</p>

        <h2>🖥️ Programming Language</h2>
        <p>This program is written in <code>C</code>.</p>

        <h2>⚙️ How It Works</h2>
        <p>The program consists of two parts:</p>
        <ul>
            <li><strong>Encryption (<code>Encrypt.c</code>)</strong>: Reads a plaintext message, encrypts it using a matrix-based key, and saves the ciphertext to a file.</li>
            <li><strong>Decryption (<code>Decrypt.c</code>)</strong>: Reads the ciphertext, computes the inverse of the key matrix, and recovers the original plaintext.</li>
        </ul>

        <h2>🧠 Main Logic</h2>
        <ol>
            <li>The user provides a <strong>2×2 or 3×3 matrix</strong> as the key.</li>
            <li>The plaintext is converted into numerical values (A=0, B=1, ..., Z=25).</li>
            <li>The message is encrypted by multiplying it with the key matrix (mod 26).</li>
            <li>The encrypted text is stored in <code>ciphertext.txt</code>.</li>
            <li>For decryption, the inverse of the key matrix is computed.</li>
            <li>The inverse matrix is used to recover the original plaintext from the ciphertext.</li>
        </ol>

        <h2>📌 Example</h2>
        <h3>Encryption</h3>
        <pre>
Input (plaintext.txt):  HELLO
Key Matrix (2×2):
1 2
3 4
Output (ciphertext.txt):  ZEBBW
        </pre>

        <h3>Decryption</h3>
        <pre>
Input (ciphertext.txt):  ZEBBW
Key Matrix (2×2):
1 2
3 4
Output (plaintext.txt):  HELLO
        </pre>

        <h2>📂 Files</h2>
        <ul>
            <li><code>Encrypt.c</code> - Encryption program</li>
            <li><code>Decrypt.c</code> - Decryption program</li>
            <li><code>plaintext.txt</code> - Input file containing the original message</li>
            <li><code>ciphertext.txt</code> - Output file containing the encrypted message</li>
        </ul>

        <h2>🚀 How to Run</h2>
        <h3>Compile the programs</h3>
        <pre>
gcc Encrypt.c -o encrypt
gcc Decrypt.c -o decrypt
        </pre>

        <h3>Run the encryption</h3>
        <pre>
./encrypt
        </pre>

        <h3>Run the decryption</h3>
        <pre>
./decrypt
        </pre>

        <div class="footer">
            <p>✨ Created by [Your Name] | 📌 GitHub: [Your GitHub Link]</p>
        </div>
    </div>
</body>
</html>
