# Steganography Script

## Description
This Python script performs basic image steganography by embedding a secret message within an image. The message is encrypted into the image and can be decrypted later using the correct passcode.

## Features
- Encrypts a secret message inside an image.
- Uses a simple mapping technique to hide message characters in pixel values.
- Requires a passcode for decryption to ensure security.

## Requirements
- Python 3.x
- OpenCV (`cv2`)

## Installation
Make sure you have Python installed on your system. You also need to install OpenCV if you haven't already:

```sh
pip install opencv-python
```

## Usage

### Encryption
1. Place the image file in the script directory and rename it to `trial_pic.jpg` (or update the script with your image filename).
2. Run the script:
   ```sh
   python stego.py
   ```
3. Enter the secret message when prompted.
4. Enter a passcode for encryption.
5. The encrypted image will be saved as `Encrypted Img.jpg` and opened automatically.

### Decryption
1. Run the script again:
   ```sh
   python stego.py
   ```
2. Enter the passcode when prompted.
3. If the passcode is correct, the hidden message will be revealed.

## Notes
- The script modifies pixel values of the image to store characters from the secret message.
- The decryption process works only if the same image and passcode are used.
- The script currently encodes only one character per pixel, limiting the message length based on image size.

## Disclaimer
This script is a simple implementation of image steganography and does not provide strong encryption. Use it for educational purposes or basic hidden messaging.

## License
This project is licensed under the MIT License.
