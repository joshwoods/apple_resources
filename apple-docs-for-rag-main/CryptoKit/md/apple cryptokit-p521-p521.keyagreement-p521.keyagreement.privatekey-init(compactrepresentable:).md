

- Apple CryptoKit
- P521
- P521.KeyAgreement
- P521.KeyAgreement.PrivateKey
-  init(compactRepresentable:) 

Initializer

# init(compactRepresentable:)

Creates a random P-521 private key for key agreement.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(compactRepresentable: Bool = true)
```

## Parameters 

`compactRepresentable`  

A Boolean value that indicates whether CryptoKit creates the key with the structure to enable compact point encoding.

## Discussion

Keys that use a compact point encoding enable shorter public keys, but aren’t compliant with FIPS certification. If your app requires FIPS certification, create a key with init(rawRepresentation:).

## See Also

### Creating a private key

init&lt;Bytes>(rawRepresentation: Bytes) throws

Creates a P-521 private key for key agreement from a collection of bytes.

init&lt;Bytes>(derRepresentation: Bytes) throws

Creates a P-521 private key for key agreement from a Distinguished Encoding Rules (DER) encoded representation.

init(pemRepresentation: String) throws

Creates a P-521 private key for key agreement from a Privacy-Enhanced Mail PEM) representation.

init&lt;Bytes>(x963Representation: Bytes) throws

Creates a P-521 private key for key agreement from an ANSI x9.63 representation.

