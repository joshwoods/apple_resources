

- Apple CryptoKit
- Curve25519
- Curve25519.Signing
- Curve25519.Signing.PrivateKey
-  signature(for:) 

Instance Method

# signature(for:)

Generates an EdDSA signature over Curve25519.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func signature(for data: D) throws -> Data where D : DataProtocol
```

## Parameters 

`data`  

The data to sign.

## Return Value

The signature for the data. Although not required by RFC 8032, which describes the Edwards-Curve Digital Signature Algorithm (EdDSA), the CryptoKit implementation of the algorithm employs randomization to generate a different signature on every call, even for the same data and key, to guard against side-channel attacks.

