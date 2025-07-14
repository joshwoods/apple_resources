

- Network Extension
- NEVPNProtocolIPSec
-  authenticationMethod 

Instance Property

# authenticationMethod

The method used to authenticate the device with the IPSec server. For IKE version 2, when using extended authentication, this authentication method only affects how the client validates the authentication payload presented by the server.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
var authenticationMethod: NEVPNIKEAuthenticationMethod { get set }
```

## Discussion

If this property is set to `NEVPNIKEAuthenticationMethodNone`, extended authentication will still be negotiated if useExtendedAuthentication is set to true.

## See Also

### Accessing IPSec properties

enum NEVPNIKEAuthenticationMethod

Internet Key Exchange (IKE) authentication methods used to authenticate with the IPSec server.

var useExtendedAuthentication: Bool

A flag indicating if extended authentication will be negotiated.

var sharedSecretReference: Data?

A persistent keychain reference to a keychain item containing the IKE shared secret.

var localIdentifier: String?

A string identifying the iOS or macOS device for authentication purposes

var remoteIdentifier: String?

A string identifying the IPSec server for authentication purposes

