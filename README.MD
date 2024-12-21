# Cipher Program

This program implements three different cipher encryption methods: ROT cipher, Affine cipher, and XOR cipher. The user can input a string and select the cipher method they wish to apply to that string. Each cipher transforms the input string according to its algorithm, and the encoded string is displayed as the result.

## Features

1. **ROT Cipher**: A substitution cipher where each letter is replaced by another letter a fixed number of positions down the alphabet. In this program, the key is set to 13, so each letter is rotated by 13 positions.

2. **Affine Cipher**: A monoalphabetic substitution cipher where each letter is transformed based on a mathematical formula. The formula used in this program is `E(x) = (ax + b) mod m`, where:
   - `a = 17`
   - `b = 20`
   - `m = 26` (number of letters in the English alphabet)

3. **XOR Cipher**: A cipher where each character is XORed with a fixed key. In this program, the XOR key is set to 5.

## Usage

1. The program will prompt the user to **Enter a string**.
2. After entering the string, the program will display the following options for cipher choice:
   - **1**: ROT Cipher
   - **2**: Affine Cipher
   - **3**: XOR Cipher
3. The user must input the choice corresponding to their desired cipher.
4. The program will then display the **encoded string** based on the selected cipher.

### Example Input and Output

- **Input**: 
Enter a string: Hello Choose cipher: 1. ROT 2. Affine 3. XOR : 1

- **Output** (ROT Cipher applied):
The encoded string is: Uryyb


---

## Code Description

### Data Section:
- `KEY`: Used for ROT cipher to shift letters by 13 positions.
- `xorKey`: The key used for XOR cipher, set to 5.
- `input_area`: Buffer for storing the input string.
- `msg_input`, `msg_output`, `msg_choice`: Messages displayed to the user.
- `a`, `b`, `m`: Parameters for the Affine cipher (`a = 17`, `b = 20`, `m = 26`).
- `xor_output`: Stores the result of the XOR cipher transformation.

### Code Flow:
1. **Input Phase**: The program asks the user to input a string.
2. **Cipher Choice**: The program prompts the user to choose one of the ciphers (ROT, Affine, XOR).
3. **Cipher Application**:
 - **ROT Cipher**: The string is encoded by rotating each character by 13 positions.
 - **Affine Cipher**: The string is encoded using the affine transformation formula.
 - **XOR Cipher**: Each character is XORed with the key (5 in this case).
4. **Output**: The transformed string is displayed to the user.

### Subroutines:
- **rotate_char**: Encodes a single character using the ROT cipher.
- **affine_cipher**: Encodes a single character using the Affine cipher.
- **xor_cipher**: Encodes a single character using the XOR cipher.

---

## Instructions

1. To run the program, assemble it with a compatible assembler (e.g., TASM or MASM).
2. Link the program and run it in a DOS emulator or real DOS environment.

---


