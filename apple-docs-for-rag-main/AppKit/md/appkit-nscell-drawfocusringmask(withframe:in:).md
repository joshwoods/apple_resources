

- AppKit
- NSCell
-  drawFocusRingMask(withFrame:in:) 

Instance Method

# drawFocusRingMask(withFrame:in:)

Draws the focus ring for the control.

macOS 10.7+

``` source
@MainActor
func drawFocusRingMask(
    withFrame cellFrame: NSRect,
    in controlView: NSView
)
```

## Parameters 

`cellFrame`  

The bounding rectangle of the receiver, or a portion of the bounding rectangle.

`controlView`  

The view that manages the cell.

## Discussion

Implemented by NSCell subclasses to draw the appropriate focus ring for the control The default implementation does nothing.

The Application Kit automatically invokes this method when appropriate, to render the view’s focus ring. The view must be eligible to become its window’s firstResponder, by overriding acceptsFirstResponder returning true.

The focus ring is rendered using the style specified by the focusRingType property, which must not be NSFocusRingType.none unless you want to suppress drawing of the focus ring. An implementation of `drawFocusRingMaskWithFrame:inView:` can assume that it is drawing in the view’s bounds, and that the fill and stroke colors have been set to an arbitrary fully opaque color. It needs only draw the desired focus ring shape or an image or other object whose outline defines the focus ring mask.

This new OS X v10.7 focus ring API should no longer call set()() and perform it’s own drawing.

## See Also

### Managing Focus Rings

func focusRingMaskBounds(forFrame: NSRect, in: NSView) -> NSRect

Returns the bounds of the focus ring mask.

class var defaultFocusRingType: NSFocusRingType

Returns the default type of focus ring for the receiver.

var focusRingType: NSFocusRingType

The type of focus ring to use with the associated view.

