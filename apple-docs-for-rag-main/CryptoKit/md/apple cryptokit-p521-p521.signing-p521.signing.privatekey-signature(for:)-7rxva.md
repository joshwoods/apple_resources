

- Apple CryptoKit
- P521
- P521.Signing
- P521.Signing.PrivateKey
-  signature(for:) 

Instance Method

# signature(for:)

Generates an Elliptic Curve Digital Signature Algorithm (ECDSA) signature of the digest you provide over the P-521 elliptic curve.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func signature(for digest: D) throws -> P521.Signing.ECDSASignature where D : Digest
```

## Parameters 

`digest`  

The digest of the data to sign.

## Return Value

The signature corresponding to the digest. The signing algorithm employs randomization to generate a different signature on every call, even for the same data and key.

## See Also

### Creating a signature

func signature&lt;D>(for: D) throws -> P521.Signing.ECDSASignature

Generates an Elliptic Curve Digital Signature Algorithm (ECDSA) signature of the data you provide over the P-521 elliptic curve, using SHA-512 as the hash function.

struct ECDSASignature

A P-521 elliptic curve digital signature algorithm (ECDSA) signature.

