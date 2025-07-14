

- Apple CryptoKit
- P521
- P521.KeyAgreement
- P521.KeyAgreement.PublicKey
-  HPKEPublicKeySerialization Implementations 

API Collection

# HPKEPublicKeySerialization Implementations

## Topics

### Initializers

init&lt;D>(D, kem: HPKE.KEM) throws

Creates a NIST P-521 elliptic curve public key for use with Diffie-Hellman key exchange.

### Instance Methods

func hpkeRepresentation(kem: HPKE.KEM) throws -> Data

Creates a serialized representation of the public key.

