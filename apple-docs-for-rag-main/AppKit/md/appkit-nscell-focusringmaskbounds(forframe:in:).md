

- AppKit
- NSCell
-  focusRingMaskBounds(forFrame:in:) 

Instance Method

# focusRingMaskBounds(forFrame:in:)

Returns the bounds of the focus ring mask.

macOS 10.7+

``` source
@MainActor
func focusRingMaskBounds(
    forFrame cellFrame: NSRect,
    in controlView: NSView
) -> NSRect
```

## Parameters 

`cellFrame`  

The bounding rectangle of the receiver, or a portion of the bounding rectangle.

`controlView`  

The view that manages the cell.

## Return Value

Returns a rectangle encompassing the focus ring bounds in the `controlView` coordinate space.

## Discussion

Implemented by `NSCell` subclasses to allow the cell to provide the rectangular bounds of the focus ring mask for the cell.

The default implementation returns an empty value. Subclasses are expected to implement this method if they intend to draw a focus ring.

## See Also

### Managing Focus Rings

func drawFocusRingMask(withFrame: NSRect, in: NSView)

Draws the focus ring for the control.

class var defaultFocusRingType: NSFocusRingType

Returns the default type of focus ring for the receiver.

var focusRingType: NSFocusRingType

The type of focus ring to use with the associated view.

