

- AppKit
- NSEvent
-  scrollingDeltaX 

Instance Property

# scrollingDeltaX

The scroll wheel’s horizontal delta.

macOS 10.7+

``` source
var scrollingDeltaX: CGFloat { get }
```

## Discussion

This is the preferred property for accessing NSScrollWheel delta values. When hasPreciseScrollingDeltas is false, your application may need to modify the raw value before using it.

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

var scrollingDeltaY: CGFloat

The scroll wheel’s vertical delta.

var momentumPhase: NSEvent.Phase

The momentum phase for a scroll or flick gesture.

var isDirectionInvertedFromDevice: Bool

A Boolean value that indicates whether the user has changed the device inversion.

