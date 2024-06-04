![Status: In Development](https://img.shields.io/badge/Status-In%20Development-blue)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

# Shift-Cipher
The **Shift Cipher**, also known as the **Caesar Cipher**, is a type of substitution cipher where each letter in the plaintext is replaced by a letter a certain number of positions further down the alphabet. This number of positions is sometimes called a **key**.
The encryption and decryption processes involve shifting the letters by a fixed number of positions, wrapping around to the beginning of the alphabet when necessary.

The encryption formula is `E_n(x) = (x + n) mod 26`, where **x** is the plaintext letter, **n** is the shift value, and **mod 26** ensures that the result is within the range of the alphabet.

The decryption formula is `D_n(x) = (x - n) mod 26`, which is the inverse of the encryption formula.

## Installation
You can install the package by cloning the repository then using pip:
```shell
git clone https://github.com/droubarka/shift-cipher.git
cd shift-cipher
python3 -m pip install .
```

Or you can use the following command instead:
```shell
pip install git+https://github.com/droubarka/shift-cipher.git
```

## Usage
As a simple usage:
```python3
from shiftcipher import shift_alpha

message = "Hello, World!"
shift = 32

encrypted_message = shift_alpha(message, shift)
decrypted_message = shift_alpha(encrypted_message, shift, reverse=True)

print(encrypted_message) # Output: "Nkrru, Cuxrj!"
print(decrypted_message) # Output: "Hello, World!"
```

## Contributing
Contributions are welcome!
If you'd like to contribute to the shift-cipher implementation,
please fork the repository and submit a pull request.

## License
The shift-cipher implementation is released under the MIT License.

[![Buy me a coffee!](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/droubarka)
