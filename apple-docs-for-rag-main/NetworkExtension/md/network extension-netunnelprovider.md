

- Network Extension
-  NETunnelProvider 

Class

# NETunnelProvider

An abstract base class shared by NEPacketTunnelProvider and NEAppProxyProvider.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NETunnelProvider
```

## Mentioned in 

Routing your VPN network traffic

## Overview

Each NETunnelProvider instance corresponds to a single tunneling session, with a single associated configuration.

Important

The `com.apple.developer.networking.networkextension` entitlement is required in order to use the NETunnelProvider class. Enable this entitlement when creating an App ID in your developer account.

### Subclassing Notes

The `NETunnelProvider` class should not be subclassed directly. Instead, you should create subclasses of `NETunnelProvider` subclasses.

#### Methods to Override

- handleAppMessage(_:completionHandler:)

## Topics

### Getting the tunnel configuration

var protocolConfiguration: NEVPNProtocol

The configuration of the current tunneling session.

var routingMethod: NETunnelProviderRoutingMethod

The method by which network traffic is routed to the tunnel.

var appRules: [NEAppRule]?

The app rules dictating which apps use the current tunneling session.

### Configuring the tunnel interface

func setTunnelNetworkSettings(NETunnelNetworkSettings?, completionHandler: (((any Error)?) -> Void)?)

Specify the network settings for the current tunneling session.

### Communicating with the containing app

func handleAppMessage(Data, completionHandler: ((Data?) -> Void)?)

Handle messages sent by the tunnel provider extension’s containing app.

### Setting tunnel status

var reasserting: Bool

Indicate to the system that the tunnel is being re-established.

### Errors

enum Code

Error codes that the tunnel provider declares.

let NETunnelProviderErrorDomain: String

The domain used for Tunnel Provider errors.

enum Code

Error codes that the tunnel provider declares.

## Relationships

### Inherits From

- NEProvider

### Inherited By

- NEAppProxyProvider
- NEPacketTunnelProvider

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### App proxy provider

class NEAppProxyProvider

The principal class for an app proxy provider app extension.

class NEProvider

An abstract base class for all NetworkExtension providers.

class NETunnelNetworkSettings

The configuration for a tunnel provider’s virtual interface.

