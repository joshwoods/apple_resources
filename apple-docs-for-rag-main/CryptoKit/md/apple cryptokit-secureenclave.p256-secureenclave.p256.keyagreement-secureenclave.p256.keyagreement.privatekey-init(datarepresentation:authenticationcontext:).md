

- Apple CryptoKit
- SecureEnclave
- 
  - SecureEnclave
- SecureEnclave.P256
- SecureEnclave.P256.KeyAgreement
- SecureEnclave.P256.KeyAgreement.PrivateKey
-  init(dataRepresentation:authenticationContext:) 

Initializer

# init(dataRepresentation:authenticationContext:)

Creates a P-256 private key for key agreement from a data representation of the key with the given authentication context.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    dataRepresentation: Data,
    authenticationContext: LAContext? = nil
) throws
```

## Parameters 

`dataRepresentation`  

A data representation of the key.

`authenticationContext`  

A local authentication context.

## See Also

### Creating a private key

init(dataRepresentation: Data) throws

Creates a P-256 private key for key agreement from the specified data representation.

init(compactRepresentable: Bool, accessControl: SecAccessControl) throws

Creates a P-256 private key for key agreement with the specified access control.

init(compactRepresentable: Bool, accessControl: SecAccessControl, authenticationContext: LAContext?) throws

Creates a P-256 private key for key agreement with the specified access control.

