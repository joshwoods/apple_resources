

- Core Media I/O
-  CMIOExtensionProvider 

Class

# CMIOExtensionProvider

An object that manages device connections for a provider.

Mac Catalyst 15.4+macOS 12.3+

``` source
class CMIOExtensionProvider
```

## Mentioned in 

Creating a camera extension with Core Media I/O

## Overview

An extension provider manages device connections and provides the startService(provider:) class method that you call to bootstrap the service.

## Topics

### Creating a Provider

init(source: any CMIOExtensionProviderSource, clientQueue: dispatch_queue_t?)

Creates an extension provider with the specified source and dispatch queue.

### Inspecting a Provider

var clientQueue: dispatch_queue_t

The dispatch queue on which the system performs client operations.

var source: (any CMIOExtensionProviderSource)?

The source for the provider.

### Starting a Provider

class func startService(provider: CMIOExtensionProvider)

Starts the system extension.

### Managing Devices

var devices: [CMIOExtensionDevice]

An array of connected devices.

func addDevice(CMIOExtensionDevice) throws

Adds a device to a provider.

func removeDevice(CMIOExtensionDevice) throws

Removes a device from a provider.

### Managing Clients

var connectedClients: [CMIOExtensionClient]

An array of connected clients.

func notifyPropertiesChanged([CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>])

Notifies connected clients of device property changes.

### Type Methods

class func ignoreSIGTERM()

class func stopService(provider: CMIOExtensionProvider)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Providers

Creating a camera extension with Core Media I/O

Build high-performance camera drivers that are secure and simple to deploy.

Overriding the default USB video class extension

Create a simple DriverKit extension to override the default driver-matching behavior for USB devices.

protocol CMIOExtensionProviderSource

A protocol for objects that act as provider sources.

class CMIOExtensionProviderProperties

An object that manages the properties of an extension provider.

