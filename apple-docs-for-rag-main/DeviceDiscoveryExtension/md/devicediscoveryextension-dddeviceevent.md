

- DeviceDiscoveryExtension
-  DDDeviceEvent 

Class

# DDDeviceEvent

An object that provides a device or communicates its change in status.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
class DDDeviceEvent
```

## Overview

The extension creates and configures an instance of this class to represent a moment of interest in the device discovery life cycle. The event’s `eventType` (DDDeviceEvent.EventType) describes a particular status.

For example, when the extension discovers a device of interest, it instantiates an instance of this class with the type DDDeviceEvent.EventType.deviceFound.

```
```

Then, the extension provides the discovered device to the system using report(_:) for eventual display in the route picker view (AVRoutePickerView).

```
```

## Topics

### Creating a device event

init(eventType: DDDeviceEvent.EventType, device: DDDevice)

Creates an event object that conveys status for a discovered device of interest.

### Configuring a device event

var eventType: DDDeviceEvent.EventType

A type for the event that describes the discovery status.

enum EventType

Identifiers for the types of events that occur in the device discovery life cycle.

var device: DDDevice

An object that describes a third-party media receiver.

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

### Life cycle

enum EventType

Identifiers for the types of events that occur in the device discovery life cycle.

func DDEventTypeToString(DDDeviceEvent.EventType) -> String

Returns human-readable text for the specified event identifier.

typealias DDEventHandler

A function that the extension invokes to signal an event.

