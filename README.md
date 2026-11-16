# Caesar Cipher | Text Encoder & Decoder

A Python implementation of the classic Caesar Cipher that encodes and decodes text by shifting letters along the alphabet

---

## Overview

The Caesar Cipher is a traditional substitution technique where every letter is moved a fixed number of positions through the alphabet. A shift of 3 turns `a` into `d`, and the alphabet wraps around so `z` leads back to `a`

This project builds the idea using only core Python: strings, lists, loops and conditions. It accepts positive and negative shift values, keeps the original letter case, and leaves spaces and punctuation untouched

I built it while learning Python, mainly to get comfortable with string handling and the modulo operator

---

## Features

- Encodes text with positive shift values
- Decodes text with negative shift values
- Handles shifts larger than 26 using modular arithmetic
- Preserves uppercase and lowercase letters
- Keeps spaces, punctuation and other symbols unchanged
- Processes several messages, each with its own shift value

---

## How It Works

The program uses a lowercase alphabet as its reference. For every character in a message, it:

1. Checks whether the character is a letter of the English alphabet
2. Finds its position in the alphabet
3. Adds the shift value
4. Applies modulo 26 so the result wraps around
5. Restores the original letter case
6. Adds the new character to the result

Anything that is not a letter is added to the result exactly as it was

---

## Example

| Original Text | Shift | Result |
|---|---:|---|
| Hello, World! | +3 | Khoor, Zruog! |
| Khoor, Zruog! | -3 | Hello, World! |
| abc | +29 | def |

**Output**

```text
Khoor, Zruog!
Hello, World!
def
```

A shift of 29 behaves like a shift of 3, because `29 % 26 = 3`
---

## Technologies & Concepts

**Language:** Python 3

**Concepts practised:**

- Variables and lists
- `for` loops and conditional statements
- String manipulation and character indexing
- `lower()`, `upper()` and `isupper()` methods
- Modular arithmetic
- Basic encoding and decoding logic

---

## Getting Started

### Requirements

- Python 3.x
- Any code editor or IDE

No external libraries are needed

### Run the Program

```bash
git clone https://github.com/Rammal-Ahmed/caesar-cipher-encoder-decoder.git
cd caesar-cipher-encoder-decoder
python caesar_cipher.py
```

To test your own text, edit the `messages` and `shifts` lists at the top of the file

---

## Project Structure

```text
caesar-cipher-encoder-decoder/
│
├── caesar_cipher.py
├── README.md
└── .gitignore
```

---

## Future Improvements

- Accept the message and shift value as user input
- Add separate encode and decode functions
- Try all 26 shifts to crack an unknown message

---

## Note

The Caesar Cipher is a learning exercise and is not suitable for protecting sensitive information

---

## About me

**Rammal Ahmed**

**AI & Data Science Enthusiast** | **Microsoft Dynamics 365 CRM Developer** | **Power Platform** | **UI/UX Designer** | **Graphic Designer & Illustrator**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/rammal-ahmed-58184b325)
[![GitHub](https://img.shields.io/badge/GitHub-Rammal--Ahmed-181717?style=flat&logo=github)](https://github.com/Rammal-Ahmed)

<div align="center">

If you found this useful, consider giving it a star ⭐

**I truly value your feedback and welcome any suggestions for improvement**

**Always open to fresh perspectives, constructive feedback, and new ideas**


## License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details

---

*Developed as part of my Python programming practice*

---

**Project Status:** Completed

</div>
