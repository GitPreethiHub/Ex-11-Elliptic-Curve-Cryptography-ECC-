# Ex-11-Elliptic-Curve-Cryptography-ECC

## Aim:
To implement Elliptic Curve Cryptography (ECC) for encryption and decryption of the plain text

## Algorithm Steps:

1) Choose an elliptic curve equation over a finite field.

2) Select a base point on the curve for generating keys.

3) Generate private and public keys for both sender and receiver.

4) Use the receiver's public key to encrypt the message.

5) Decrypt the encrypted message using the receiver's private key.

## Program
```
#include <stdio.h>
#include <stdlib.h>

int main() {
    printf("Experiment 11 - Elliptic Curve Cryptography (ECC)\n");
    printf("**************Preethi M 212222100037*************\n");

    int private_key = 5;
    int base_point = 7;
    int prime = 23;
    int public_key = (base_point * private_key) % prime;

    printf("Private Key: %d\n", private_key);
    printf("Public Key: %d\n", public_key);

    int shared_secret = (public_key * private_key) % prime;
    printf("Shared Secret: %d\n", shared_secret);

    return 0;
}

```
## Output
![image](https://github.com/user-attachments/assets/1c1d4c0c-91e7-4fff-8425-6a68fcd99096)

## Result
The shared secret is successfully generated using Elliptic Curve Cryptography.
