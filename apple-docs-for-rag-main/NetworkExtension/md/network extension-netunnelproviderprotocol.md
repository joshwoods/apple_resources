

- Network Extension
-  NETunnelProviderProtocol 

Class

# NETunnelProviderProtocol

Configuration parameters for a VPN tunnel.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NETunnelProviderProtocol
```

## Overview

`NETunnelProviderProtocol` objects are used to specify configuration parameters for Tunnel Provider extensions.

## Topics

### Accessing the tunnel configuration

var providerConfiguration: [String : Any]?

A dictionary containing keys and values defined by the Tunnel Provider developer.

var providerBundleIdentifier: String?

A string identifying the specific Tunnel Provider extension that should be used with this configuration.

## Relationships

### Inherits From

- NEVPNProtocol

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

class NEAppProxyProviderManager

An object to create and manage the app proxy provider’s VPN configuration.

class NETunnelProviderManager

An object to create and manage the tunnel provider’s VPN configuration.

class NEVPNManager

An object to create and manage a Personal VPN configuration.

class NEAppRule

The identity of an app whose traffic is to be routed through the tunnel.

VPN On Demand Rules

Set up VPN On Demand.

