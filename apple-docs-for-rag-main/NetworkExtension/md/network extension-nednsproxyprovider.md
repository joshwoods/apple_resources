

- Network Extension
-  NEDNSProxyProvider 

Class

# NEDNSProxyProvider

The principal class for a DNS proxy provider app extension.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class NEDNSProxyProvider
```

## Mentioned in 

Handling Flow Copying

## Overview

A DNS proxy allows your app to intercept all DNS traffic generated on a device. You can use this capability to provide services like DNS traffic encryption, typically by redirecting DNS traffic to your own server. You usually do this in the context of managed devices, such as those owned by a school or an enterprise.

You create a DNS proxy as an app extension based on a custom subclass of the NEDNSProxyProvider class. Once active, the proxy receives access to flows of DNS traffic in the form of NEAppProxyFlow instances. Each flow corresponds to a socket opened by an app to UDP port 53 or TCP port 53. Your DNS proxy provider acts as a transparent DNS proxy for the flows of network data that it receives.

Important

To use the NEDNSProxyProvider class, you must enable the Network Extensions capability in Xcode and select the DNS Proxy capability. See Configure network extensions.

When you subclass NEDNSProxyProvider, you must provide implementations for the following methods:

- startProxy(options:completionHandler:)

- stopProxy(with:completionHandler:)

- handleNewFlow(_:)

## Topics

### Managing the DNS proxy life cycle

func startProxy(options: [String : Any]?, completionHandler: ((any Error)?) -> Void)

Starts the DNS proxy.

func stopProxy(with: NEProviderStopReason, completionHandler: () -> Void)

Stops the DNS proxy.

func cancelProxyWithError((any Error)?)

Cancels the DNS proxy.

### Handling proxied DNS flow

func handleNewFlow(NEAppProxyFlow) -> Bool

Handles a new flow of DNS traffic.

func handleNewUDPFlow(NEAppProxyUDPFlow, initialRemoteEndpoint: NWEndpoint) -> Bool

Handles a new flow of UDP traffic.

Deprecated

### Getting system DNS settings

var systemDNSSettings: [NEDNSSettings]?

The current system DNS settings.

## Relationships

### Inherits From

- NEProvider

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Provider

class NEDNSSettings

The DNS resolver settings of a network tunnel or a system-wide configuration.

