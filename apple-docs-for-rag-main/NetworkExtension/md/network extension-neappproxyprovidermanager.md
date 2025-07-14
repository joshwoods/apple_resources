

- Network Extension
-  NEAppProxyProviderManager 

Class

# NEAppProxyProviderManager

An object to create and manage the app proxy provider’s VPN configuration.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
class NEAppProxyProviderManager
```

## Mentioned in 

Routing your VPN network traffic

## Overview

Objects cannot be directly instantiated. Instead, App Proxy configurations are created exclusively from `com.apple.vpn.managed.applayer` payloads in configuration profiles.

App Proxy configurations can only be used with Per-App VPN routing rules. For more details about how to create App Proxy configurations and configure Per-App VPN, see NETunnelProviderManager.

Important

The `com.apple.developer.networking.networkextension` entitlement is required in order to use the NEAppProxyProviderManager class. Enable this entitlement when creating an App ID in your developer account.

## Topics

### Loading the app proxy configuration

class func loadAllFromPreferences(completionHandler: ([NEAppProxyProviderManager]?, (any Error)?) -> Void)

Load all of the App Proxy configurations associated with the calling app that have previously been saved to the Network Extension preferences.

## Relationships

### Inherits From

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

class NETunnelProviderManager

An object to create and manage the tunnel provider’s VPN configuration.

class NEVPNManager

An object to create and manage a Personal VPN configuration.

class NETunnelProviderProtocol

Configuration parameters for a VPN tunnel.

class NEAppRule

The identity of an app whose traffic is to be routed through the tunnel.

VPN On Demand Rules

Set up VPN On Demand.

