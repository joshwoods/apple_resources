

- AppKit
- NSClipView
-  scroll(to:) 

Instance Method

# scroll(to:)

Changes the origin of the clip view’s bounds rectangle to `newOrigin`.

macOS

``` source
@MainActor
func scroll(to newOrigin: NSPoint)
```

## See Also

### Scrolling

func autoscroll(with: NSEvent) -> Bool

Scrolls the clip view proportionally to `theEvent`’s distance outside of it.

func constrainScroll(NSPoint) -> NSPoint

Returns a scroll point adjusted from the proposed new origin, if necessary, to guarantee the view will lie within its document view.

Deprecated

func constrainBoundsRect(NSRect) -> NSRect

Constrains the bounds of the clip view while the user is magnifying and scrolling.

