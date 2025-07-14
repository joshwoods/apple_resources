

- AppKit
- NSCell
-  defaultFocusRingType 

Type Property

# defaultFocusRingType

Returns the default type of focus ring for the receiver.

macOS

``` source
@MainActor
class var defaultFocusRingType: NSFocusRingType { get }
```

## Return Value

The default type of focus ring for the receiver (one of the values listed in NSFocusRingType).

## See Also

### Managing Focus Rings

func drawFocusRingMask(withFrame: NSRect, in: NSView)

Draws the focus ring for the control.

func focusRingMaskBounds(forFrame: NSRect, in: NSView) -> NSRect

Returns the bounds of the focus ring mask.

var focusRingType: NSFocusRingType

The type of focus ring to use with the associated view.

