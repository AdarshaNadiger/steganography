# steganography
This project demonstrates image steganography using Least Significant Bit (LSB) encoding and decoding in C. It allows you to hide secret messages inside an image and retrieve them later.

Features
LSB Encoding: Embed a text message into the least significant bits of image pixels.
LSB Decoding: Extract the hidden message from an image.
Written in C without external libraries (uses standard C file I/O).
Works with BMP images for simplicity.

How It Works
Encoding:
Each character of the message is converted to binary.
Each bit of the message is hidden in the LSB of the image's pixel color values (commonly RGB).

Decoding:
Extracts the LSBs of image pixels to reconstruct the hidden binary message.
Converts binary back to readable text.
