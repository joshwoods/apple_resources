

- Apple CryptoKit
- Curve25519
- Curve25519.Signing
- Curve25519.Signing.PublicKey
-  isValidSignature(\_:for:) 

Instance Method

# isValidSignature(\_:for:)

Verifies an EdDSA signature over Curve25519.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func isValidSignature(
    _ signature: S,
    for data: D
) -> Bool where S : DataProtocol, D : DataProtocol
```

## Parameters 

`signature`  

The signature to check against the given data.

`data`  

The data covered by the signature.

## Return Value

A Boolean value that’s `true` when the signature is valid for the given data.

