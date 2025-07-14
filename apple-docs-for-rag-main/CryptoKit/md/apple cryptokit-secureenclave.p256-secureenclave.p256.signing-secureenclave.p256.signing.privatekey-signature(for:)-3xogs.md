

- Apple CryptoKit
- SecureEnclave
- 
  - SecureEnclave
- SecureEnclave.P256
- SecureEnclave.P256.Signing
- SecureEnclave.P256.Signing.PrivateKey
-  signature(for:) 

Instance Method

# signature(for:)

Generates an Elliptic Curve Digital Signature Algorithm (ECDSA) signature of the digest you provide over the P-256 elliptic curve.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func signature(for digest: D) throws -> P256.Signing.ECDSASignature where D : Digest
```

## Parameters 

`digest`  

The digest of the data to sign.

## Return Value

The signature corresponding to the digest. The signing algorithm employs randomization to generate a different signature on every call, even for the same digest and key.

## See Also

### Generating a signature

func signature&lt;D>(for: D) throws -> P256.Signing.ECDSASignature

Generates an elliptic curve digital signature algorithm (ECDSA) signature of the given data over the P-256 elliptic curve, using SHA-256 as the hash function.

