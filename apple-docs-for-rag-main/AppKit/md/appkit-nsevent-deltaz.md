

- AppKit
- NSEvent
-  deltaZ 

Instance Property

# deltaZ

The z-coordinate change for a scroll wheel, mouse-move, or mouse-drag event.

macOS

``` source
var deltaZ: CGFloat { get }
```

## Discussion

This value is typically `0.0`.

## See Also

### Getting scroll wheel and flick events

var deltaX: CGFloat

The x-coordinate change for scroll wheel, mouse-move, mouse-drag, and swipe events.

var deltaY: CGFloat

The y-coordinate change for scroll wheel, mouse-move, mouse-drag, and swipe events.

var hasPreciseScrollingDeltas: Bool

A Boolean value that indicates whether precise scrolling deltas are available.

var scrollingDeltaX: CGFloat

The scroll wheel’s horizontal delta.

var scrollingDeltaY: CGFloat

The scroll wheel’s vertical delta.

var momentumPhase: NSEvent.Phase

The momentum phase for a scroll or flick gesture.

var isDirectionInvertedFromDevice: Bool

A Boolean value that indicates whether the user has changed the device inversion.

