

- AppKit
- NSClipView
-  constrainBoundsRect(\_:) 

Instance Method

# constrainBoundsRect(\_:)

Constrains the bounds of the clip view while the user is magnifying and scrolling.

macOS 10.9+

``` source
@MainActor
func constrainBoundsRect(_ proposedBounds: NSRect) -> NSRect
```

## Parameters 

`proposedBounds`  

The bounds to use to ensure that the view will still lie within its document view.

## Return Value

A bounds rectangle.

## Discussion

Note that you can move an implementation of the deprecated constrainScroll(_:) to this method by adjusting the origin of `proposedBounds` (instead of using the `newOrigin` parameter in `-constrainScrollPoint:`). To preserve compatibility, if a subclass overrides `-constrainScrollPoint:`, the default behavior of constrainBoundsRect(_:) will be to use that `-constrainScrollPoint:` to adjust the origin of `proposedBounds`, and to not change the size.

## See Also

### Scrolling

func scroll(to: NSPoint)

Changes the origin of the clip view’s bounds rectangle to `newOrigin`.

func autoscroll(with: NSEvent) -> Bool

Scrolls the clip view proportionally to `theEvent`’s distance outside of it.

func constrainScroll(NSPoint) -> NSPoint

Returns a scroll point adjusted from the proposed new origin, if necessary, to guarantee the view will lie within its document view.

Deprecated

