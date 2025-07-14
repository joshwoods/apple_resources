

- DeviceDiscoveryExtension
-  DDEventHandler 

Type Alias

# DDEventHandler

A function that the extension invokes to signal an event.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
typealias DDEventHandler = (DDDeviceEvent) -> Void
```

## Parameters 

`inEvent`  

An event that the extension creates for the event handler.

## Discussion

A device discovery extension implements a closure of this format and calls it after creating argument events. In the implementation, the extension creates device events (`DDEvent`) and passes them to the system by calling report(_:).

For an example event handler, see `Appex.swift` in Discovering a third-party media-streaming device.

## See Also

### Life cycle

class DDDeviceEvent

An object that provides a device or communicates its change in status.

enum EventType

Identifiers for the types of events that occur in the device discovery life cycle.

func DDEventTypeToString(DDDeviceEvent.EventType) -> String

Returns human-readable text for the specified event identifier.

