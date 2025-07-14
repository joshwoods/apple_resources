

- Network Extension
-  NEVPNManager 

Class

# NEVPNManager

An object to create and manage a Personal VPN configuration.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEVPNManager
```

## Overview

The NEVPNManager API gives apps the ability to create and manage a Personal VPN configuration on iOS and macOS. Personal VPN configurations are typically used to provide a service to users that protects their Internet browsing activity on insecure networks such as public Wi-Fi networks.

## Topics

### Managing VPN configurations

class func shared() -> NEVPNManager

Access the single instance of `NEVPNManager`.

func loadFromPreferences(completionHandler: ((any Error)?) -> Void)

Load the VPN configuration from the Network Extension preferences.

func saveToPreferences(completionHandler: (((any Error)?) -> Void)?)

Save the VPN configuration in the Network Extension preferences.

func setAuthorization(AuthorizationRef)

func removeFromPreferences(completionHandler: (((any Error)?) -> Void)?)

Remove the VPN configuration from the Network Extension preferences.

### Accessing VPN configuration properties

var isEnabled: Bool

A Boolean used to toggle the enabled state of the VPN configuration.

var protocolConfiguration: NEVPNProtocol?

An NEVPNProtocol object containing the configuration settings of the VPN tunneling protocol.

var `protocol`: NEVPNProtocol?

An `NEVPNProtocol` object containing the configuration settings of the VPN tunneling protocol.

Deprecated

var localizedDescription: String?

A string containing the display name of the VPN configuration.

var isOnDemandEnabled: Bool

A Boolean used to toggle the Connect On Demand capability.

var onDemandRules: [NEOnDemandRule]?

An ordered list of Connect On Demand rules.

### Connecting and disconnecting VPN

var connection: NEVPNConnection

An NEVPNConnection object that is used to control the VPN tunnel specified by the VPN configuration.

### Errors

enum Code

Codes that indicate the source of an error.

let NEVPNErrorDomain: String

enum Code

Codes that indicate the source of an error.

### Notifications

static let NEVPNConfigurationChange: NSNotification.Name

Posted after the VPN configuration stored in the Network Extension preferences changes.

### Entitlements

Personal VPN Entitlement

The API an app can use to create and control a custom system VPN configuration.

## Relationships

### Inherits From

- NSObject

### Inherited By

- NETransparentProxyManager
- NETunnelProviderManager

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### VPN configuration

class NEAppProxyProviderManager

An object to create and manage the app proxy provider’s VPN configuration.

class NETunnelProviderManager

An object to create and manage the tunnel provider’s VPN configuration.

class NETunnelProviderProtocol

Configuration parameters for a VPN tunnel.

class NEAppRule

The identity of an app whose traffic is to be routed through the tunnel.

VPN On Demand Rules

Set up VPN On Demand.

