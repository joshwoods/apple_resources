

- External Accessory
-  EAAccessory 

Class

# EAAccessory

An object that contains information about a single, connected hardware accessory.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
class EAAccessory
```

## Overview

An EAAccessory object gives your app information about a single connected hardware accessory. You can use the information in this class to determine whether your app is able to open a session to a given accessory. After you have an open session, you can also associate a custom delegate with the accessory object to be notified to changes in the accessory state. Your delegate must adopt the EAAccessoryDelegate protocol.

You use an accessory object to create an EASession object, which itself provides the communications channel to and from the accessory hardware. The accessory object provides information about the communications protocols the accessory supports, along with information about current hardware and firmware revisions.

When deciding whether to connect to an accessory, you should always first check the accessory’s declared protocols in the protocolStrings array. This list indicates the types of data the accessory is capable of processing at that moment, which may not be the full list of protocols for which the accessory is designed. For example, an accessory that is connected but not yet authenticated will report no supported protocols until authentication is successful. Don’t connect to the accessory unless and until the list includes the protocol you intend to use.

Accessories can be physically connected to the device through the Lightning connector (or through the 30-pin connector on older devices) or wirelessly using Bluetooth.

## Topics

### Responding to Disconnection Events

var delegate: (any EAAccessoryDelegate)?

The object that acts as the delegate of the accessory.

protocol EAAccessoryDelegate

A protocol that defines an optional method for receiving notifications when the associated accessory object is disconnected.

### Getting Connection Information

var isConnected: Bool

A Boolean value indicating whether the accessory is currently connected to the iOS-based device.

var connectionID: Int

The accessory’s unique ID for connecting to the iOS-based device.

Null Connection ID

The ID for an unconnected accessory.

### Getting the Manufacturer-Supplied Attributes

var name: String

The display name of the accessory.

var manufacturer: String

The name of the accessory’s manufacturer.

var modelNumber: String

The model information for the accessory.

var serialNumber: String

The serial number of the accessory.

var firmwareRevision: String

The current firmware version for the accessory.

var hardwareRevision: String

The hardware version of the accessory.

var protocolStrings: [String]

The communication protocols supported by the accessory.

var dockType: StringDeprecated

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

### Accessory Communication

class EASession

The object you use to manage communications between your app and a connected hardware accessory.

