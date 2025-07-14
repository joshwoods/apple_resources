

- Security
- Certificate, Key, and Trust Services
- Identities
-  Storing an Identity in the Keychain 

Article

# Storing an Identity in the Keychain

Securely store an identity in the keychain.

## Overview

You store an identity in or retrieve an identity from a keychain much as you would a certificate, as described in Storing a Certificate in the Keychain.

Private keys have a one-to-many relationship with certificates. That is, a single private key can be paired with multiple certificates, but a given certificate corresponds to exactly one private key. As a result, the fields that distinguish one identity from another are the same as those of the certificate it contains. As a result, working with identities as keychain items is very much like working with certificates, with a few minor adjustments:

- Use SecIdentity objects instead of SecCertificate objects.

- Use kSecClassIdentity instead of kSecClassCertificate for the kSecClass attribute.

