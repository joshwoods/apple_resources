

- Apple CryptoKit
- SecureEnclave
- 
  - SecureEnclave
- SecureEnclave.P256
- SecureEnclave.P256.KeyAgreement
- SecureEnclave.P256.KeyAgreement.PrivateKey
-  init(compactRepresentable:accessControl:authenticationContext:) 

Initializer

# init(compactRepresentable:accessControl:authenticationContext:)

Creates a P-256 private key for key agreement with the specified access control.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    compactRepresentable: Bool = true,
    accessControl: SecAccessControl = SecAccessControlCreateWithFlags(nil, kSecAttrAccessibleAfterFirstUnlockThisDeviceOnly, [], nil)!,
    authenticationContext: LAContext? = nil
) throws
```

## Parameters 

`compactRepresentable`  

A Boolean value that indicates whether CryptoKit creates the key with the structure to enable compact point encoding.

`accessControl`  

The protection type and flags to use when creating the associated access control object.

`authenticationContext`  

A local authentication context.

## See Also

### Creating a private key

init(dataRepresentation: Data) throws

Creates a P-256 private key for key agreement from the specified data representation.

init(dataRepresentation: Data, authenticationContext: LAContext?) throws

Creates a P-256 private key for key agreement from a data representation of the key with the given authentication context.

init(compactRepresentable: Bool, accessControl: SecAccessControl) throws

Creates a P-256 private key for key agreement with the specified access control.

