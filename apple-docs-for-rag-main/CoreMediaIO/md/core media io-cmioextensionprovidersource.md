

- Core Media I/O
-  CMIOExtensionProviderSource 

Protocol

# CMIOExtensionProviderSource

A protocol for objects that act as provider sources.

Mac Catalyst 15.4+macOS 12.3+

``` source
protocol CMIOExtensionProviderSource : NSObjectProtocol
```

## Overview

Create a class that adopts this protocol to configure provider properties and manage its client connections.

## Topics

### Managing Connections

func connect(to: CMIOExtensionClient) throws

Connects a client to a source’s provider.

**Required**

func disconnect(from: CMIOExtensionClient)

Disconnects a client from a source’s provider.

**Required**

### Configuring Properties

var availableProperties: Set&lt;CMIOExtensionProperty>

A set of available properties for a provider.

**Required**

func providerProperties(forProperties: Set&lt;CMIOExtensionProperty>) throws -> CMIOExtensionProviderProperties

Gets the state of provider properties.

**Required**

func setProviderProperties(CMIOExtensionProviderProperties) throws

Set the state of provider properties.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Providers

Creating a camera extension with Core Media I/O

Build high-performance camera drivers that are secure and simple to deploy.

Overriding the default USB video class extension

Create a simple DriverKit extension to override the default driver-matching behavior for USB devices.

class CMIOExtensionProvider

An object that manages device connections for a provider.

class CMIOExtensionProviderProperties

An object that manages the properties of an extension provider.

