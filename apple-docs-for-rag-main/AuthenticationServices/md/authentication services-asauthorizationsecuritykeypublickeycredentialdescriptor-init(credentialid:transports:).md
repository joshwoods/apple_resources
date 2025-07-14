

- Authentication Services
- ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor
-  init(credentialID:transports:) 

Initializer

# init(credentialID:transports:)

Creates the object with the credential ID and the array of transports.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(
    credentialID: Data,
    transports allowedTransports: [ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor.Transport]
)
```

## Parameters 

`credentialID`  

The credential identifier.

`allowedTransports`  

The array of allowed transports.

## See Also

### Creating the descriptor

var transports: [ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor.Transport]

The array of transport types.

struct Transport

A structure that defines the security key credential transport type.

