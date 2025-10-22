# Caesar Cipher 🔐

Python implementation of the classic Caesar cipher encryption algorithm.

## Features
- Encrypt text with custom shift value
- Decrypt encrypted messages
- Supports both uppercase and lowercase letters
- Validates shift parameter (1-25)

## How to use

### Encrypt
```python
from caesar_cipher import encrypt

text = "Hello World"
encrypted = encrypt(text, 13)
print(encrypted)  # "Uryyb Jbeyq"
```

### Decrypt
```python
from caesar_cipher import decrypt

encrypted_text = "Uryyb Jbeyq"
decrypted = decrypt(encrypted_text, 13)
print(decrypted)  # "Hello World"
```

## Example
The program includes an example that decrypts:
```
"Pbhentr vf sbhaq va hayvxryl cynprf."
```
Using ROT13 (shift of 13) to reveal the hidden message.

## Technologies
- Python 3.x
- String manipulation
- `str.maketrans()` and `translate()` methods

## Algorithm
The Caesar cipher shifts each letter in the alphabet by a fixed number of positions. For example, with a shift of 3:
- A → D
- B → E
- C → F
