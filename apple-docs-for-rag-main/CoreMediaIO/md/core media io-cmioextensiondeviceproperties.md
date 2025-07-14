

- Core Media I/O
-  CMIOExtensionDeviceProperties 

Class

# CMIOExtensionDeviceProperties

An object that defines the properties of a device.

Mac Catalyst 15.4+macOS 12.3+

``` source
class CMIOExtensionDeviceProperties
```

## Overview

Create an instance of this object to manage the device’s property state.

## Topics

### Creating Device Properties

init(dictionary: [CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>])

Creates a properties object with a dictionary of property states.

### Configuring Device Properties

var model: String?

A device model string.

var linkedCoreAudioDeviceUID: String?

A universal identifier of the audio device linked to this device.

var transportType: Int?

The transport type of the device, such as USB or HDMI.

var suspended: Bool?

A Boolean value that indicates whether the device is in a suspended state.

func setPropertyState(CMIOExtensionPropertyState&lt;AnyObject>?, forProperty: CMIOExtensionProperty)

Sets the value of a device property.

var propertiesDictionary: [CMIOExtensionProperty : CMIOExtensionPropertyState&lt;AnyObject>]

A dictionary of properties for a device.

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

class CMIOExtensionDevice

An object that represents a physical or virtual device.

protocol CMIOExtensionDeviceSource

A protocol for objects that act as device sources.

