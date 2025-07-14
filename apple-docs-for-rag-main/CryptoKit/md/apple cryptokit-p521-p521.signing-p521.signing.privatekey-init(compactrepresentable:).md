

- Apple CryptoKit
- P521
- P521.Signing
- P521.Signing.PrivateKey
-  init(compactRepresentable:) 

Initializer

# init(compactRepresentable:)

Creates a random P-521 private key for signing.

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

### Creating a key

init&lt;Bytes>(rawRepresentation: Bytes) throws

Creates a P-521 private key for signing from a collection of bytes.

init&lt;Bytes>(derRepresentation: Bytes) throws

Creates a P-521 private key for signing from a Distinguished Encoding Rules (DER) encoded representation.

init(pemRepresentation: String) throws

Creates a P-521 private key for signing from a Privacy-Enhanced Mail PEM) representation.

init&lt;Bytes>(x963Representation: Bytes) throws

Creates a P-521 private key for signing from an ANSI x9.63 representation.

