

- Network Extension
-  NEVPNProtocolIPSec 

Class

# NEVPNProtocolIPSec

Settings for an IPsec VPN configuration.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEVPNProtocolIPSec
```

## Overview

To configure IKE version 2 (IKEv2), use the NEVPNProtocolIKEv2 subclass. Instantiating NEVPNProtocolIPSec directly implies IKE version 1.

## Topics

### Accessing IPSec properties

var authenticationMethod: NEVPNIKEAuthenticationMethod

The method used to authenticate the device with the IPSec server. For IKE version 2, when using extended authentication, this authentication method only affects how the client validates the authentication payload presented by the server.

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

## Relationships

### Inherits From

- NEVPNProtocol

### Inherited By

- NEVPNProtocolIKEv2

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### VPN configuration

class NEVPNManager

An object to create and manage a Personal VPN configuration.

class NEVPNProtocolIKEv2

Settings for an IKEv2 VPN configuration.

class NEVPNProtocol

Settings common to both IKEv2 and IPsec VPN configurations.

VPN On Demand Rules

Set up VPN On Demand.

