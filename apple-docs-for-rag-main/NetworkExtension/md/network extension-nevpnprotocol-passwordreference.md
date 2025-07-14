

- Network Extension
- NEVPNProtocol
-  passwordReference 

Instance Property

# passwordReference

A persistent keychain reference to a keychain item containing the password component of the tunneling protocol authentication credential.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var passwordReference: Data? { get set }
```

## Discussion

The keychain item must have the kSecClassGenericPassword class.

## See Also

### Authenticating the user

var username: String?

The user name component of the tunneling protocol authentication credential.

var identityReference: Data?

A persistent keychain reference to a keychain item containing the certificate and private key components of the tunneling protocol authentication credential.

var identityData: Data?

The certificate and private key components of the tunneling protocol authentication credential, in PKCS12 format.

var identityDataPassword: String?

The password for the PKCS12 tunneling protocol authentication credentials.

