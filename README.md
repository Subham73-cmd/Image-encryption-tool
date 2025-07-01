# Image Encryption and Decryption Tool

A simple Python script for **image encryption and decryption** using pixel manipulation with the Pillow (PIL) library. This tool swaps the red and blue channels of each pixel to "encrypt" the image, and applies the same operation to "decrypt" it back to the original.

## Features

- Encrypts an image by swapping RGB channels (red ↔ blue)
- Decrypts the image using the same logic
- Works with any standard image format supported by Pillow
- Minimal dependencies, easy to understand and extend

## How It Works

- **Encryption:** For every pixel, the red and blue values are swapped.
- **Decryption:** The same swap is applied, restoring the original image.
- This is a reversible, demonstrative method and **not secure for real-world cryptography**.

## Requirements

- Python 3.x
- [Pillow (PIL)](https://pypi.org/project/Pillow/)

## Installation

```bash
pip install Pillow
```

## Usage

1. **Edit the file paths** in the script to point to your input and output images.
2. **Run the script:**
    ```bash
    python image_encrypt_decrypt.py
    ```
3. The script will:
    - Encrypt the input image and save it as the encrypted image.
    - Decrypt the encrypted image and save it as the decrypted image.

## Example

```python
input_image = r"C:\path\to\original_image.jpeg"
encrypted_image = r"C:\path\to\encrypted_image.jpeg"
decrypted_image = r"C:\path\to\decrypted_image.jpeg"

encrypt_image(input_image, encrypted_image, key=None)
decrypt_image(encrypted_image, decrypted_image, key=None)
```

## Notes

- This method is for learning and demonstration purposes only.
- For real-world image security, use strong cryptographic algorithms such as AES[1][2].
- You can extend the script to use more sophisticated encryption methods if needed.


**Educational Use Only — Not for Secure Applications**
