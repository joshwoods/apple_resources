

- Network Extension
-  NEProvider 

Class

# NEProvider

An abstract base class for all NetworkExtension providers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
class NEProvider
```

## Overview

See the documentation for the `NEProvider` subclasses for details about how to create Network Extension Provider extensions.

The `NEProvider` class and its subclasses expose methods and properties that allow Network Extension Provider extensions to participate in and affect the network data path on iOS and macOS. For example, the `handleNewFlow:` method in NEFilterDataProvider allows Filter Data Provider extensions to make pass/block decisions on TCP connections as the connections are established on the system.

### Subclassing Notes

The `NEProvider` class should not be subclassed directly. Instead, you should create subclasses of `NEProvider` subclasses (and in some cases subsubclasses).

#### Methods to Override

- sleep(completionHandler:)

- wake()

## Topics

### Handling sleep and wake

func sleep(completionHandler: () -> Void)

Handle a sleep event.

func wake()

Handle a wake event.

### Creating network connections

func createTCPConnection(to: NWEndpoint, enableTLS: Bool, tlsParameters: NWTLSParameters?, delegate: Any?) -> NWTCPConnection

Create a TCP connection.

Deprecated

func createUDPSession(to: NWEndpoint, from: NWHostEndpoint?) -> NWUDPSession

Creates a UDP session.

Deprecated

### Monitoring the network state

var defaultPath: NWPath?

The current default network path used for connections created by the provider.

Deprecated

### Supporting system extensions

class func startSystemExtensionMode()

Starts the Network Extension machinery from inside a System Extension.

### Constants

enum NEProviderStopReason

Reasons why the provider extension was stopped.

### Displaying messages

func displayMessage(String, completionHandler: (Bool) -> Void)

Call this method from your NEProvider subclass if you want to display a message to the person using the app.

Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- NEAppPushProvider
- NEDNSProxyProvider
- NEFilterProvider
- NETunnelProvider

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

class NETunnelProvider

An abstract base class shared by NEPacketTunnelProvider and NEAppProxyProvider.

class NETunnelNetworkSettings

The configuration for a tunnel provider’s virtual interface.

