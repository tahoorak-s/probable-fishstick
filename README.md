# SecureFile – AES-256 File Encryption Tool


## Overview

SecureFile is a Python-based file encryption and decryption tool implemented in Google Colab. It uses AES-256 encryption with CBC mode to securely encrypt and decrypt files. The application supports any file type and provides an easy-to-use interface with upload and download features directly within the Colab environment.

---

## Features

* **AES-256 encryption and decryption** using `pycryptodome`
* **Password-based key derivation** with PBKDF2 and random salt
* **Encrypt/decrypt any file format** (text, PDF, images, etc.)
* **Secure password input** (hidden input)
* **Upload files from local machine to Colab**
* **Download encrypted/decrypted files directly from Colab**

---

## How to Use

1. **Open the Colab notebook** and run the setup cell to install dependencies.
2. Run the encryption/decryption functions definition cell.
3. Run the menu cell:

   * Upload your file when prompted.
   * Enter the password (input will be hidden).
   * Choose whether to encrypt or decrypt.
4. The processed file will be downloaded automatically to your local machine.

   * Encrypted files have the `.enc` extension.
   * Decrypted files have the `.dec` extension.

---

## Dependencies

* Python 3.x
* `pycryptodome` (installed automatically via pip in the notebook)
* `google.colab` (built-in in Google Colab)

---

## Notes

* This tool is designed to run **only in Google Colab**.
* File encryption uses **AES-256 in CBC mode** with random IV and salt.
* Passwords are processed securely using PBKDF2 key derivation with 100,000 iterations.
* Always keep your password safe; losing it means losing access to your encrypted data.

---

## Sample Usage

```python
# Run menu function and follow prompts:
colab_menu()
```

---

