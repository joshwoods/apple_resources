

- DeviceDiscoveryExtension
-  DDEventTypeToString(\_:) 

Function

# DDEventTypeToString(\_:)

Returns human-readable text for the specified event identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOSvisionOS 1.0+

``` source
func DDEventTypeToString(_ inValue: DDDeviceEvent.EventType) -> String
```

## Parameters 

`inValue`  

An event identifier to convert to text.

## Return Value

A textual value for the specified event type.

## Discussion

Your extension can use this function for logging.

## See Also

### Life cycle

class DDDeviceEvent

An object that provides a device or communicates its change in status.

enum EventType

Identifiers for the types of events that occur in the device discovery life cycle.

typealias DDEventHandler

A function that the extension invokes to signal an event.

