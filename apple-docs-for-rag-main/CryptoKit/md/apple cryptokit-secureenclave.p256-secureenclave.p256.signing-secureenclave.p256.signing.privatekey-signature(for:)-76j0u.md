

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

Generates an elliptic curve digital signature algorithm (ECDSA) signature of the given data over the P-256 elliptic curve, using SHA-256 as the hash function.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func signature(for data: D) throws -> P256.Signing.ECDSASignature where D : DataProtocol
```

## Parameters 

`data`  

The data to sign.

## Return Value

A cryptographic signature. The signing algorithm employs randomization to generate a different signature on every call, even for the same data and key.

## See Also

### Generating a signature

func signature&lt;D>(for: D) throws -> P256.Signing.ECDSASignature

Generates an Elliptic Curve Digital Signature Algorithm (ECDSA) signature of the digest you provide over the P-256 elliptic curve.

