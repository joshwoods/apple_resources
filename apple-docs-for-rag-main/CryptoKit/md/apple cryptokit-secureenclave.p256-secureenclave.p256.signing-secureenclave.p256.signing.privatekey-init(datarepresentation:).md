

- Apple CryptoKit
- SecureEnclave
- 
  - SecureEnclave
- SecureEnclave.P256
- SecureEnclave.P256.Signing
- SecureEnclave.P256.Signing.PrivateKey
-  init(dataRepresentation:) 

Initializer

# init(dataRepresentation:)

Creates a P-256 private key for signing from the specified data representation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
init(dataRepresentation: Data) throws
```

## Parameters 

`dataRepresentation`  

A data representation of the key.

## See Also

### Creating a private key

init(dataRepresentation: Data, authenticationContext: LAContext?) throws

Creates a P-256 private key for signing from a data representation of the key with the given authentication context.

init(compactRepresentable: Bool, accessControl: SecAccessControl) throws

Creates a P-256 private key for signing with the specified access control.

init(compactRepresentable: Bool, accessControl: SecAccessControl, authenticationContext: LAContext?) throws

Creates a P-256 private key for signing with the specified access control.

