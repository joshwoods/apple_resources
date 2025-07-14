

- Network Extension
- NEVPNProtocol
-  identityData 

Instance Property

# identityData

The certificate and private key components of the tunneling protocol authentication credential, in PKCS12 format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var identityData: Data? { get set }
```

## Discussion

In macOS, the system ignores this property for NEVPNProtocolIKEv2 and NETunnelProviderProtocol objects. On iOS, the system ignores this property for NETunnelProviderProtocol objects. In cases where the system ignores this property, set the identity using the identityReference property.

## See Also

### Authenticating the user

var username: String?

The user name component of the tunneling protocol authentication credential.

var passwordReference: Data?

A persistent keychain reference to a keychain item containing the password component of the tunneling protocol authentication credential.

var identityReference: Data?

A persistent keychain reference to a keychain item containing the certificate and private key components of the tunneling protocol authentication credential.

var identityDataPassword: String?

The password for the PKCS12 tunneling protocol authentication credentials.

