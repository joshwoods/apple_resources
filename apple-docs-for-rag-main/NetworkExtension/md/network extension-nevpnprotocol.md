

- Network Extension
-  NEVPNProtocol 

Class

# NEVPNProtocol

Settings common to both IKEv2 and IPsec VPN configurations.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEVPNProtocol
```

## Mentioned in 

Routing your VPN network traffic

## Overview

The NEVPNProtocol class is an abstract base class with one subclass for each type of supported VPN configuration. This class provides properties for configuring the VPN, authenticating network connections, and routing network traffic. You can include all network traffic, with some exceptions, and selectively exclude types of network traffic.

Instances of this class are thread-safe.

## Topics

### Configuring the VPN

var serverAddress: String?

The address of the VPN server.

var disconnectOnSleep: Bool

A Boolean value that indicates whether the VPN disconnects when the device sleeps.

var proxySettings: NEProxySettings?

The proxy settings to use for HTTP and HTTPS connections that route through the VPN.

### Authenticating the user

var username: String?

The user name component of the tunneling protocol authentication credential.

var passwordReference: Data?

A persistent keychain reference to a keychain item containing the password component of the tunneling protocol authentication credential.

var identityReference: Data?

A persistent keychain reference to a keychain item containing the certificate and private key components of the tunneling protocol authentication credential.

var identityData: Data?

The certificate and private key components of the tunneling protocol authentication credential, in PKCS12 format.

var identityDataPassword: String?

The password for the PKCS12 tunneling protocol authentication credentials.

### Routing network traffic

var includeAllNetworks: Bool

A Boolean value that indicates whether the system sends most network traffic over the tunnel.

var excludeAPNs: Bool

A Boolean value that indicates whether the system excludes all APNs network traffic from the tunnel.

var excludeCellularServices: Bool

A Boolean value that indicates whether the system excludes all cellular services network traffic from the tunnel.

var excludeLocalNetworks: Bool

A Boolean value that indicates whether the system excludes all traffic destined for local networks from the tunnel.

var enforceRoutes: Bool

A Boolean value that indicates whether route rules for the tunnel take precedence over any locally defined routes.

### Instance Properties

var excludeDeviceCommunication: Bool

var sliceUUID: String?

## Relationships

### Inherits From

- NSObject

### Inherited By

- NEDNSProxyProviderProtocol
- NETunnelProviderProtocol
- NEVPNProtocolIPSec

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

class NEVPNProtocolIPSec

Settings for an IPsec VPN configuration.

VPN On Demand Rules

Set up VPN On Demand.

