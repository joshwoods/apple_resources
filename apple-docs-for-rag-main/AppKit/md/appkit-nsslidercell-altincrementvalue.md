

- AppKit
- NSSliderCell
-  altIncrementValue 

Instance Property

# altIncrementValue

The amount by which the slider changes its value when the user Option-drags the knob.

macOS

``` source
@MainActor
var altIncrementValue: Double { get set }
```

## Discussion

By default, the value of this property is -1.0, and the slider behaves no differently with the Option key down than with it up. If you set this property, the number should correspond to the range of values the slider can represent—for example, if the slider has a minimum value of 5 and a maximum value of 10, the value should be between 0 and 5.

## See Also

### Related Documentation

Slider Programming Topics

### Managing Cell Behavior

class var prefersTrackingUntilMouseUp: Bool

Returns a Boolean value indicating whether the `NSSliderCell` continues to track the pointer until the next mouse up.

var trackRect: NSRect

The rectangle within which the cell tracks the pointer while the mouse button is down.

