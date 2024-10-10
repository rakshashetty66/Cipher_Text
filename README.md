# Cipher Text Encryption and Decryption
This Python project implements a simple Caesar Cipher algorithm to encrypt and decrypt messages using a predefined alphabet. The Caesar Cipher is a basic substitution cipher where each letter in the plaintext is shifted by a specified number of positions in the alphabet to produce the cipher text. Similarly, during decryption, the letters in the cipher text are shifted back to their original positions using the same key.

# Features:
1. Encryption: Converts a plaintext message into cipher text by shifting the letters by a given number (shift key).
2. Decryption: Recovers the original plaintext message from cipher text using the same shift key.
3. User input prompts guide through the process of encryption or decryption.
4. Alphabet:
The cipher operates on the lowercase English alphabet:
['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']

# Step-by-Step Workflow:
1. Encryption Function:

The encryption(plain_text, shift_key) function takes two inputs:
plain_text: The original message that you want to encrypt.
shift_key: The number of positions to shift each letter in the alphabet.
Process:

For each letter in plain_text, the function:
Finds the position of the letter in the alphabet.
Shifts the letter by shift_key positions to find the new letter.
Modulus operation ensures the alphabet wraps around (e.g., 'z' shifts to 'a').
The new letter is appended to cipher_text.
Finally, the encrypted message is printed.

2. Decryption Function:
The decryption(cipher_text, shift_key) function reverses the process:

Takes the cipher_text and the same shift_key used during encryption.
For each letter in cipher_text:
Finds its position in the alphabet.
Shifts the letter back by shift_key positions to get the original letter.
Modulus operation ensures proper wrapping around the alphabet.
The original letter is appended to plain_text.
Finally, the decrypted message is printed.

3. Main Program Loop:
The program prompts the user for the following inputs:

Encrypt or Decrypt: Choose to either encrypt or decrypt a message.
Text Input: Enter the message for encryption or decryption.
Shift Key: Enter a numeric shift key for the cipher.
Based on the input, the program either encrypts or decrypts the message using the respective function.

After each operation, the user is asked whether they want to continue:

Type 'yes' to perform another encryption/decryption.
Type 'no' to exit the program with a friendly goodbye message.
