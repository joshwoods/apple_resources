

- AppKit
- NSEvent
-  hasPreciseScrollingDeltas 

Instance Property

# hasPreciseScrollingDeltas

A Boolean value that indicates whether precise scrolling deltas are available.

macOS 10.7+

``` source
var hasPreciseScrollingDeltas: Bool { get }
```

## Discussion

This property is set to true if precise scrolling deltas are available; otherwise, false.

This property is valid for NSScrollWheel events. A generic scroll wheel issues rather coarse scroll deltas. Some mice and trackpads provide much more precise delta. This method determines how the values of the scrollingDeltaX and scrollingDeltaY should be interpreted.

## See Also

### Getting scroll wheel and flick events

var deltaX: CGFloat

The x-coordinate change for scroll wheel, mouse-move, mouse-drag, and swipe events.

var deltaY: CGFloat

The y-coordinate change for scroll wheel, mouse-move, mouse-drag, and swipe events.

var deltaZ: CGFloat

The z-coordinate change for a scroll wheel, mouse-move, or mouse-drag event.

var scrollingDeltaX: CGFloat

The scroll wheel’s horizontal delta.

var scrollingDeltaY: CGFloat

The scroll wheel’s vertical delta.

var momentumPhase: NSEvent.Phase

The momentum phase for a scroll or flick gesture.

var isDirectionInvertedFromDevice: Bool

A Boolean value that indicates whether the user has changed the device inversion.

