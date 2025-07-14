

- AppKit
- NSEvent
-  deltaY 

Instance Property

# deltaY

The y-coordinate change for scroll wheel, mouse-move, mouse-drag, and swipe events.

macOS

``` source
var deltaY: CGFloat { get }
```

## Discussion

This property is only valid for scroll wheel, mouse-move, mouse-drag, and swipe events. For swipe events, a nonzero value represents a horizontal swipe; `-1.0` corresponds to swipe down and `1.0` corresponds to swipe up.

For scroll wheel events, use scrollingDeltaY instead.

## See Also

### Getting scroll wheel and flick events

var deltaX: CGFloat

The x-coordinate change for scroll wheel, mouse-move, mouse-drag, and swipe events.

var deltaZ: CGFloat

The z-coordinate change for a scroll wheel, mouse-move, or mouse-drag event.

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

