

- AppKit
- NSCell
-  focusRingType 

Instance Property

# focusRingType

The type of focus ring to use with the associated view.

macOS

``` source
@MainActor
var focusRingType: NSFocusRingType { get set }
```

## Discussion

You can disable a view’s focus ring drawing by setting this property to NSFocusRingType.none. The only times you should disable focus ring drawing are when you want to draw your own focus ring or when there is insufficient space to display a focus ring in the default location.

## See Also

### Managing Focus Rings

func drawFocusRingMask(withFrame: NSRect, in: NSView)

Draws the focus ring for the control.

func focusRingMaskBounds(forFrame: NSRect, in: NSView) -> NSRect

Returns the bounds of the focus ring mask.

class var defaultFocusRingType: NSFocusRingType

Returns the default type of focus ring for the receiver.

