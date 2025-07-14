

- PassKit (Apple Pay and Wallet)
- Apple Pay
- Payment token format reference
-  Restoring the symmetric key 

Article

# Restoring the symmetric key

Restore the symmetric key you use to verify payment data.

## Overview

The value of the `version` key in the payment token structure indicates whether the Apple Pay servers encrypted the payment token using Elliptic Curve Cryptography (ECC) or Rivest–Shamir–Adleman (RSA). Follow the instructions for restoring an ECC key or an RSA key according to the value of the `version` key.

For instructions on using the symmetric key, see Payment token format reference.

### Restore a symmetric key for ECC

To restore the key for ECC (`EC_v1)`, follow these steps:

1.  Use the merchant private key and the ephemeral public key to generate the shared secret using Elliptic Curve Diffie-Hellman (id-ecDH 1.3.132.1.12).

2.  Use the merchant identifier field (OID 1.2.840.113635.100.6.32) of the public key certificate and the shared secret to derive the symmetric key using the key derivation function described in NIST SP 800-56A, section 5.8.1, with the input values shown in the following table:

| Input Name | Value |
|----|----|
| Z | SHA-256 |
| Algorithm ID | The shared secret calculated above using ECDH. |
| Party U Info | The ASCII string `"Apple"`. This value is a fixed-length string. |
| Party V Info | The SHA-256 hash of your merchant ID string literal, which is 32 bytes in size.  You can derive Party V Info from your payment processing certificate in either of two ways.  Method 1:  The UID field of the Common Name includes the plaintext merchant ID. Calculate the SHA-256 hash of that plaintext string. Use the result for Party V Info.  Method 2:  The OID 1.2.840.113635.100.6.32 includes the hex-encoded hash of the merchant ID . Hexadecimal-decode that hash string to produce the original (non-hex-encoded) 32-byte hash. Use the result for Party V Info. |
| Supplemental Public and Private Info | Unused |

### Restore a symmetric key for RSA

A merchant’s public key encrypts the symmetric key for RSA (`RSA_v1)` by using the RSA/ECB/OAEPWithSHA256AndMGF1Padding algorithm. Use your RSA private key to decrypt the cipher text in the `wrappedKey` value. After you decrypt it, the plaintext is the symmetric key material that you use to decrypt the payment token.

