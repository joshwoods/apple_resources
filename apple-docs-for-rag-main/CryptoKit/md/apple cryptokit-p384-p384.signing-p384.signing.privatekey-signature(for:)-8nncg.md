

- Apple CryptoKit
- P384
- P384.Signing
- P384.Signing.PrivateKey
-  signature(for:) 

Instance Method

# signature(for:)

Generates an Elliptic Curve Digital Signature Algorithm (ECDSA) signature of the data you provide over the P-384 elliptic curve, using SHA-384 as the hash function.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func signature(for data: D) throws -> P384.Signing.ECDSASignature where D : DataProtocol
```

## Parameters 

`data`  

The data to sign.

## Return Value

The signature corresponding to the data. The signing algorithm employs randomization to generate a different signature on every call, even for the same data and key.

## See Also

### Creating a signature

func signature&lt;D>(for: D) throws -> P384.Signing.ECDSASignature

Generates an Elliptic Curve Digital Signature Algorithm (ECDSA) signature of the digest you provide over the P-384 elliptic curve.

struct ECDSASignature

A P-384 elliptic curve digital signature algorithm (ECDSA) signature.

