

- Authentication Services
- ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor
-  transports 

Instance Property

# transports

The array of transport types.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var transports: [ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor.Transport] { get set }
```

## See Also

### Creating the descriptor

init(credentialID: Data, transports: [ASAuthorizationSecurityKeyPublicKeyCredentialDescriptor.Transport])

Creates the object with the credential ID and the array of transports.

struct Transport

A structure that defines the security key credential transport type.

