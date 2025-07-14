

- AppKit
- NSClipView
-  constrainScroll(\_:) Deprecated

Instance Method

# constrainScroll(\_:)

Returns a scroll point adjusted from the proposed new origin, if necessary, to guarantee the view will lie within its document view.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func constrainScroll(_ newOrigin: NSPoint) -> NSPoint
```

Deprecated

Use constrainBoundsRect(_:) instead.

## Parameters 

`newOrigin`  

Origin proposed.

## Return Value

A point which will guarantee the view will lie within its document view.

## Discussion

For example, if the x-coordinate of `newOrigin` lies to the left of the document view’s origin, then the x-coordinate returned is set to that of the x-coordinate of the document view’s origin.

## See Also

### Scrolling

func scroll(to: NSPoint)

Changes the origin of the clip view’s bounds rectangle to `newOrigin`.

func autoscroll(with: NSEvent) -> Bool

Scrolls the clip view proportionally to `theEvent`’s distance outside of it.

func constrainBoundsRect(NSRect) -> NSRect

Constrains the bounds of the clip view while the user is magnifying and scrolling.

