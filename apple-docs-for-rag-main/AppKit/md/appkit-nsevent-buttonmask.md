

- AppKit
- NSEvent
-  buttonMask 

Instance Property

# buttonMask

A bit mask identifying the buttons pressed for a tablet event.

macOS

``` source
var buttonMask: NSEvent.ButtonMask { get }
```

## Discussion

Use one or more of the button-mask constants described in `Getting Unicode Values` to determine which of the pointing device’s buttons are pressed. This property is valid only for mouse events with a subtype of `NSTabletPointEventSubtype` and for events of type `NSTabletPoint`; otherwise, the property is set to `0`.

## See Also

### Getting tablet pointing information

var absoluteX: Int

The absolute x coordinate of a pointing device on its tablet at full tablet resolution.

var absoluteY: Int

The absolute y coordinate of a pointing device on its tablet at full tablet resolution.

var absoluteZ: Int

The absolute z coordinate of pointing device on its tablet at full tablet resolution.

struct ButtonMask

Constants you use to identify the activated tablet buttons in an event.

var rotation: Float

The rotation in degrees of the tablet pointing device associated with this event.

var tangentialPressure: Float

The tangential pressure on the device that generated this event.

var tilt: NSPoint

The scaled tilt values of the pointing device that generated this event.

var vendorDefined: Any

An array of three vendor-defined number objects associated with a pointing-type event.

