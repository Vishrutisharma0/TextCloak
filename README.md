 ## TextCloak
 The Text Cloak Website is a web-based application that allows users to encrypt and decrypt messages.
 The application has been developed by using both cryptography and steganography.The secret message will be hidden inside another text, the cover message. The secret message encrypted using password can be embedded in the cover message by the sender, extracted from the cover message, and decrypted using the same password by the receiver.

## Functions implemented
- Embed algorithm: To embed the secret message into the cover message by converting it into invisible zero width unicode characters.
- Extract algorithm: To extract the secret message from the cover message by converting it back into ascii characters from invisible zero width unicode characters.
- AES-encryption: We take the password for encrypting the secret message before embedding it,the key for encryption is generated from the password-based key derivation function PBKDF2.
- AES-decryption: For decryption, we need to pass the same password used while encryption since AES-256 is a symmetric cipher.

## Tech stack
- Backend : Python3, Flask
- Frontend : Html, CSS

## Screenshots
- Enter secret message to be sent, cover message and password.
  
![tc1](https://github.com/Vishrutisharma0/TextCloak/assets/83419687/3ff6c45c-523b-4e93-9e70-5d00b6a30038)

- On clicking the Hide button, the cover message with an embedded secret message is displayed and copied to the clipboard.

![tc2](https://github.com/Vishrutisharma0/TextCloak/assets/83419687/3665ee8f-2f34-46be-8d34-83e5ee4e6d19)

- Enter the received embedded cover message in the "Stegcloaked Message" field and mutually decided password in the "Password" field. After clicking on the Get Secret button the secret message will be displayed.
  
![tc3](https://github.com/Vishrutisharma0/TextCloak/assets/83419687/52b16fc9-4012-47ba-84a3-ee7ee9db2e7f)

## Installation

Install the dependency for AES by running:
- pip install pycryptodomex




				
			



