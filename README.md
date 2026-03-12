# 🔐 Caesar Cipher — Custom Alphabet (a-z / 0-9)

**Text encryption, decryption, frequency analysis, and shift detection in Python.**  
The project reads text from `.txt` files, writes results to `.txt` files, uses a custom alphabet consisting of **letters + digits**, and leaves **Polish diacritics / special characters unchanged**.

---

## 🎯 Goal
This project focuses on:
- encrypting text with a **Caesar-style shift cipher**,
- decrypting text using a selected shift,
- analyzing character frequencies for the custom alphabet,
- finding the most likely shift for an encrypted text using a **reference text**.

---

## 🧠 Cipher rules
### 🔹 Custom alphabet
The cipher uses the following alphabet:

```text
abcdefghijklmnopqrstuvwxyz0123456789
```

### 🔹 Supported characters
The program transforms:
- lowercase English letters `a-z`
- digits `0-9`

### 🔹 Unchanged characters
The following characters remain unchanged:
- Polish letters: `ą ć ę ł ń ó ś ź ż`
- spaces
- punctuation
- line breaks
- all other characters outside the custom alphabet

### 🔹 Letter handling
Uppercase and lowercase letters are treated as the same during processing.  
The output is saved in **lowercase**.

---

## ⚙️ Project features
- file-based encryption and decryption,
- frequency analysis of letters and digits,
- shift detection based on frequency comparison,
- support for both:
  - **English version** of the script,
  - **Polish version** of the script.

---

## 📂 Repository structure
```text
.
├─ maineng.py
├─ mainpl.py
├─ README.md
├─ LICENSE
├─ .gitignore
├─ input.txt
├─ output.txt
├─ reference.txt
├─ encrypted.txt
├─ decrypted.txt
├─ analysis.txt
└─ ranking.txt
```

---

## ▶️ Running the project

Run the English version:
```bash
python maineng.py
```

Run the Polish version:
```bash
python mainpl.py
```

---

## 🧪 Program options
The program provides three main functions:

### 1. Encrypt / decrypt a file
- reads text from a `.txt` file,
- encrypts or decrypts it using a given shift,
- saves the result to another `.txt` file.

### 2. Character frequency analysis
- counts how many times each character from the custom alphabet appears,
- calculates the percentage share of each character,
- ignores spaces, punctuation, and other unsupported symbols.

### 3. Find shift and decrypt
- compares an encrypted text with a reference text,
- checks all possible shifts,
- selects the shift with the smallest frequency difference,
- saves the decrypted result and ranking to files.

---

## 📄 Example files
Suggested example files for testing:
- `input.txt` — plain text to encrypt
- `reference.txt` — reference text for frequency comparison
- `encrypted.txt` — encrypted text
- `decrypted.txt` — recovered plaintext
- `analysis.txt` — frequency report
- `ranking.txt` — list of shifts sorted by similarity

---

## ✨ Notes
- This project implements a **Caesar / shift cipher**, not a transposition cipher.
- Characters outside the custom alphabet are preserved exactly as they appear.
- The project is intended as an **educational Python exercise** for text processing, file handling, and basic cryptography concepts.

---

### 🧑‍💻 Author
Created by **Avuii**
