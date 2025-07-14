

- Network Extension
-  NEVPNIKEAuthenticationMethod 

Enumeration

# NEVPNIKEAuthenticationMethod

Internet Key Exchange (IKE) authentication methods used to authenticate with the IPSec server.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
enum NEVPNIKEAuthenticationMethod
```

## Topics

### Authentication methods

case none

Do not authenticate with the IPSec server. Note that extended authentication may still be performed if the useExtendedAuthentication property is set. This value is only valid for IKE version 2 (IKEv2)

case certificate

Use a certificate and private key as the authentication credential. The certificate and private key set in the identityReference or identityData property will be used.

case sharedSecret

Use a shared secret as the authentication credential. The shared secret set in the sharedSecretReference property will be used.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing IPSec properties

var authenticationMethod: NEVPNIKEAuthenticationMethod

The method used to authenticate the device with the IPSec server. For IKE version 2, when using extended authentication, this authentication method only affects how the client validates the authentication payload presented by the server.

var useExtendedAuthentication: Bool

A flag indicating if extended authentication will be negotiated.

var sharedSecretReference: Data?

A persistent keychain reference to a keychain item containing the IKE shared secret.

var localIdentifier: String?

A string identifying the iOS or macOS device for authentication purposes

var remoteIdentifier: String?

A string identifying the IPSec server for authentication purposes

