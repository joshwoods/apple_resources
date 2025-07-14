

- Network Extension
-  NEAppRule 

Class

# NEAppRule

The identity of an app whose traffic is to be routed through the tunnel.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
class NEAppRule
```

## Topics

### Initializing an app rule

init(signingIdentifier: String)

Create an app rule that matches an app with a given signing identifier.

init(signingIdentifier: String, designatedRequirement: String)

Create an app rule that matches an app with a given signing identifier and a given designated requirement.

### Accessing app rule properties

var matchSigningIdentifier: String

The signing identifier of the app that matches the rule.

var matchDesignatedRequirement: String

The designated requirement of the app that matches the rule.

var matchPath: String?

The file system path of the app that matches the rule.

var matchDomains: [Any]?

The hostname domains that match the rule.

var matchTools: [NEAppRule]?

An array of app rule objects that restrict the rule so it only matches network traffic generated from helper processes.

## Relationships

### Inherits From

- NSObject

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

class NETunnelProviderProtocol

Configuration parameters for a VPN tunnel.

VPN On Demand Rules

Set up VPN On Demand.

