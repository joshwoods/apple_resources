

- AppKit
- NSEvent
-  vendorDefined 

Instance Property

# vendorDefined

An array of three vendor-defined number objects associated with a pointing-type event.

macOS

``` source
var vendorDefined: Any { get }
```

## Discussion

This property contains an array of three NSNumber objects. Each object encapsulates a `short` value that vendors may return for various reasons; see the vendor documentation for details.This method is valid for mouse events with subtype NSTabletPointEventSubtype and for NSTabletPoint events.

## See Also

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

var tilt: NSPoint

The scaled tilt values of the pointing device that generated this event.

