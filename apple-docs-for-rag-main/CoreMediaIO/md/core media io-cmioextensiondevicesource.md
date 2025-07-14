

- Core Media I/O
-  CMIOExtensionDeviceSource 

Protocol

# CMIOExtensionDeviceSource

A protocol for objects that act as device sources.

Mac Catalyst 15.4+macOS 12.3+

``` source
protocol CMIOExtensionDeviceSource : NSObjectProtocol
```

## Overview

Create a class that adopts this protocol to configure device properties.

## Topics

### Managing Properties

var availableProperties: Set&lt;CMIOExtensionProperty>

A set of available properties that a device provides.

**Required**

func deviceProperties(forProperties: Set&lt;CMIOExtensionProperty>) throws -> CMIOExtensionDeviceProperties

Retrieves the state of device properties.

**Required**

func setDeviceProperties(CMIOExtensionDeviceProperties) throws

Sets the state of device properties.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Devices

class CMIOExtensionDevice

An object that represents a physical or virtual device.

class CMIOExtensionDeviceProperties

An object that defines the properties of a device.

