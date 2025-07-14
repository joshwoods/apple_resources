

- Apple CryptoKit
- SecureEnclave
- 
  - SecureEnclave
- SecureEnclave.P256
- SecureEnclave.P256.KeyAgreement
- SecureEnclave.P256.KeyAgreement.PrivateKey
-  DiffieHellmanKeyAgreement Implementations 

API Collection

# DiffieHellmanKeyAgreement Implementations

## Topics

### Instance Methods

func sharedSecretFromKeyAgreement(with: P256.KeyAgreement.PublicKey) throws -> SharedSecret

Computes a shared secret with the provided public key from another party.

