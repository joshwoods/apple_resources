

- AppKit
- NSEvent
-  scrollingDeltaY 

Instance Property

# scrollingDeltaY

The scroll wheel’s vertical delta.

macOS 10.7+

``` source
var scrollingDeltaY: CGFloat { get }
```

## Discussion

This is the preferred property for accessing NSScrollWheel delta values. When hasPreciseScrollingDeltas is false, multiply the value returned by this method by the line or row height. Otherwise scroll by the returned amount.

## See Also

### Getting scroll wheel and flick events

var deltaX: CGFloat

The x-coordinate change for scroll wheel, mouse-move, mouse-drag, and swipe events.

var deltaY: CGFloat

The y-coordinate change for scroll wheel, mouse-move, mouse-drag, and swipe events.

var deltaZ: CGFloat

The z-coordinate change for a scroll wheel, mouse-move, or mouse-drag event.

var hasPreciseScrollingDeltas: Bool

A Boolean value that indicates whether precise scrolling deltas are available.

var scrollingDeltaX: CGFloat

The scroll wheel’s horizontal delta.

var momentumPhase: NSEvent.Phase

The momentum phase for a scroll or flick gesture.

var isDirectionInvertedFromDevice: Bool

A Boolean value that indicates whether the user has changed the device inversion.

