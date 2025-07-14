

- Core Media I/O
-  CMIOExtensionDevice 

Class

# CMIOExtensionDevice

An object that represents a physical or virtual device.

Mac Catalyst 15.4+macOS 12.3+

``` source
class CMIOExtensionDevice
```

## Mentioned in 

Creating a camera extension with Core Media I/O

## Overview

A device provides one or more streams of media data to a CMIOExtensionProvider.

## Topics

### Creating a Device

convenience init(localizedName: String, deviceID: UUID, source: any CMIOExtensionDeviceSource)

Creates an extension device.

init(localizedName: String, deviceID: UUID, legacyDeviceID: String?, source: any CMIOExtensionDeviceSource)

Creates an extension device with an optional legacy device identifier.

### Identifying a Device

var localizedName: String

A localized name for a device.

var deviceID: UUID

A universally unique device identifier value.

var legacyDeviceID: String

A legacy device identifier.

### Managing Streams

var streams: [CMIOExtensionStream]

An array of media streams attached to this device.

func addStream(CMIOExtensionStream) throws

Adds a stream to a device.

func removeStream(CMIOExtensionStream) throws

Removes a stream from the device.

### Accessing the Device Source

var source: (any CMIOExtensionDeviceSource)?

A source object for a device.

### Posting Property Changes

func notifyPropertiesChanged([CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>])

Notifies clients of property changes.

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

### Devices

protocol CMIOExtensionDeviceSource

A protocol for objects that act as device sources.

class CMIOExtensionDeviceProperties

An object that defines the properties of a device.

