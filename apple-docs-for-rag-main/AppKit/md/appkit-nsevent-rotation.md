

- AppKit
- NSEvent
-  rotation 

Instance Property

# rotation

The rotation in degrees of the tablet pointing device associated with this event.

macOS

``` source
var rotation: Float { get }
```

## Discussion

Many devices do not support rotation, in which case the returned value is 0.0. This property is valid only for mouse events with subtype `NSTabletPointEventSubtype` and for `NSTabletPoint` events.

## See Also

### Related Documentation

var pressure: Float

A normalized value that indicates the degree of pressure applied to an appropriate input device.

### Getting tablet pointing information

var absoluteX: Int

The absolute x coordinate of a pointing device on its tablet at full tablet resolution.

var absoluteY: Int

The absolute y coordinate of a pointing device on its tablet at full tablet resolution.

var absoluteZ: Int

The absolute z coordinate of pointing device on its tablet at full tablet resolution.

var buttonMask: NSEvent.ButtonMask

A bit mask identifying the buttons pressed for a tablet event.

struct ButtonMask

Constants you use to identify the activated tablet buttons in an event.

var tangentialPressure: Float

The tangential pressure on the device that generated this event.

var tilt: NSPoint

The scaled tilt values of the pointing device that generated this event.

var vendorDefined: Any

An array of three vendor-defined number objects associated with a pointing-type event.

