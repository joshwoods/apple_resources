

- Network Extension
- NEVPNProtocol
-  identityDataPassword 

Instance Property

# identityDataPassword

The password for the PKCS12 tunneling protocol authentication credentials.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var identityDataPassword: String? { get set }
```

## Discussion

If the PKCS12 data set in the identityData property uses a password for encryption, you must specify the password here.

## See Also

### Authenticating the user

var username: String?

The user name component of the tunneling protocol authentication credential.

var passwordReference: Data?

A persistent keychain reference to a keychain item containing the password component of the tunneling protocol authentication credential.

var identityReference: Data?

A persistent keychain reference to a keychain item containing the certificate and private key components of the tunneling protocol authentication credential.

var identityData: Data?

The certificate and private key components of the tunneling protocol authentication credential, in PKCS12 format.

