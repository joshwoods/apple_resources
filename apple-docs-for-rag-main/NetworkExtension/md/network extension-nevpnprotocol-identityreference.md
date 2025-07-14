

- Network Extension
- NEVPNProtocol
-  identityReference 

Instance Property

# identityReference

A persistent keychain reference to a keychain item containing the certificate and private key components of the tunneling protocol authentication credential.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var identityReference: Data? { get set }
```

## Discussion

The keychain item must have the kSecClassIdentity class. In macOS, the system ignores this property for NEVPNProtocolIPSec objects. On iOS, the system ignores this property for NEVPNProtocolIPSec and NEVPNProtocolIKEv2 objects. In these cases where the system ingores this property, set the identity using the identityData property.

## See Also

### Authenticating the user

var username: String?

The user name component of the tunneling protocol authentication credential.

var passwordReference: Data?

A persistent keychain reference to a keychain item containing the password component of the tunneling protocol authentication credential.

var identityData: Data?

The certificate and private key components of the tunneling protocol authentication credential, in PKCS12 format.

var identityDataPassword: String?

The password for the PKCS12 tunneling protocol authentication credentials.

