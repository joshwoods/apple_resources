

- AppKit
- NSSliderCell
-  trackRect 

Instance Property

# trackRect

The rectangle within which the cell tracks the pointer while the mouse button is down.

macOS

``` source
@MainActor
var trackRect: NSRect { get }
```

## Discussion

The tracking rectangle includes the slider bar, but not the bezel.

## See Also

### Managing Cell Behavior

var altIncrementValue: Double

The amount by which the slider changes its value when the user Option-drags the knob.

class var prefersTrackingUntilMouseUp: Bool

Returns a Boolean value indicating whether the `NSSliderCell` continues to track the pointer until the next mouse up.

