

- AppKit
- NSEvent
-  tilt 

Instance Property

# tilt

The scaled tilt values of the pointing device that generated this event.

macOS

``` source
var tilt: NSPoint { get }
```

## Discussion

This property’s value can range from -1.0 to 1.0 for both axes. A negative x-coordinate value indicates a tilt to the left and a positive value indicates a tilt to the right; a negative y-coordinate value indicates a tilt to the top and a positive value indicates a tilt to the bottom. If the device is perfectly perpendicular to the table surface, the values are 0.0 for both axes. This property is valid for mouse events with subtype `NSTabletPointEventSubtype` and for `NSTabletPoint` events.

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

var rotation: Float

The rotation in degrees of the tablet pointing device associated with this event.

var tangentialPressure: Float

The tangential pressure on the device that generated this event.

var vendorDefined: Any

An array of three vendor-defined number objects associated with a pointing-type event.

