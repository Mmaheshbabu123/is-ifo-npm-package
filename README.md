# Encrypt Decrypt Service

A simple encryption and decryption service using AES-256 with CryptoJS.

## Installation

```bash
npm i ifo-encrypt-decrypt-js
```
#USAGE
```jsx
import EncryptDecryptService from 'ifo-encrypt-decrypt-js';


// Encrypt data
const encrypted = EncryptDecryptService.encryptData({ foo: 'bar' });
console.log('Encrypted:', encrypted);

// Decrypt data
const decrypted = EncryptDecryptService.decryptData(encrypted);
console.log('Decrypted:', decrypted);
```
Using Custom Key and IV from Environment Variables

By default, the package comes with built-in keys for AES encryption. However, you can specify your own custom AES key and IV through environment variables.

In your .env file, set the following:
```bash
AES_KEY="your-custom-32-character-aes-key" # Must be 32 characters long for AES-256
AES_IV="your-custom-16-character-aes-iv"   # Must be 16 characters long for the IV

```



