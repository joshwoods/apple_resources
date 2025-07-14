

- DeviceDiscoveryExtension
- DDDeviceEvent
-  DDDeviceEvent.EventType 

Enumeration

# DDDeviceEvent.EventType

Identifiers for the types of events that occur in the device discovery life cycle.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
enum EventType
```

## Overview

An event (`DDEvent`) `eventType` is of this type.

## Topics

### Distinguishing event types

case unknown

A value for uninitialized event types.

case deviceFound

A status that indicates when the extension finds the device of interest.

case deviceLost

A status that indicates when the extension loses a connection to the device of interest.

case deviceChanged

A status that indicates when the device of interest changes configuration.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Life cycle

class DDDeviceEvent

An object that provides a device or communicates its change in status.

func DDEventTypeToString(DDDeviceEvent.EventType) -> String

Returns human-readable text for the specified event identifier.

typealias DDEventHandler

A function that the extension invokes to signal an event.

