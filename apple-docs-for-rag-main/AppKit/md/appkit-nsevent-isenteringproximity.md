

- AppKit
- NSEvent
-  isEnteringProximity 

Instance Property

# isEnteringProximity

A Boolean value that indicates whether a pointing device is entering or leaving the proximity of its tablet.

macOS

``` source
var isEnteringProximity: Bool { get }
```

## Discussion

This property is set to true when the pointing device enters the proximity of its tablet and false when it leaves.

This method is valid only for mouse events with subtype `NSTabletProximityEventSubtype` and for `NSTabletProximity` events; otherwise it is set to false.

## See Also

### Getting tablet proximity information

var capabilityMask: Int

A mask that indicates the capabilities of the tablet device that generated this event.

var deviceID: Int

A special identifier the system matches against tablet-pointer and tablet-proximity events.

var pointingDeviceID: Int

The index of the pointing device currently in proximity with the tablet.

var pointingDeviceSerialNumber: Int

The vendor-assigned serial number of a pointing device.

var pointingDeviceType: NSEvent.PointingDeviceType

The kind of pointing device associated with this event.

enum PointingDeviceType

The pointing-device types for tablet-proximity events or mouse events with a proximity event subtype.

var systemTabletID: Int

The index of the tablet device connected to the system.

var tabletID: Int

The USB model identifier of the tablet device associated with this event.

var uniqueID: UInt64

The unique identifier of the pointing device that generated this event.

var vendorID: Int

The vendor identifier of the tablet associated with the event.

var vendorPointingDeviceType: Int

A coded bit field whose set bits indicate the type of pointing device (within a vendor selection) associated with the event.

