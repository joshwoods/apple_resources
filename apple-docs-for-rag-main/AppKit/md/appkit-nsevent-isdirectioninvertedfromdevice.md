

- AppKit
- NSEvent
-  isDirectionInvertedFromDevice 

Instance Property

# isDirectionInvertedFromDevice

A Boolean value that indicates whether the user has changed the device inversion.

macOS 10.7+

``` source
var isDirectionInvertedFromDevice: Bool { get }
```

## Discussion

This property is set to true if the direction is inverted; otherwise, false.

This property is valid for `NSEventScrollWheel` and NSEvent.EventType.swipe events. The user may choose to change the scrolling behavior such that it feels like they are moving the content instead of the scroll bar.

To accomplish this, deltaX and deltaY and scrollingDeltaX and scrollingDeltaY values are automatically inverted for NSEventScrollWheel events according to the user’s preferences.

The direction of fluid swipes matches the direction of scrolling and as such for NSEventTypeSwipe events gestureAmount is inverted. However, for some uses of NSEventScrollWheel and NSEventTypeSwipe events, the behavior should not respect the user preference. This property allows you to determine when the event has been inverted and compensate by multiplying by `-1` if needed.

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

var scrollingDeltaY: CGFloat

The scroll wheel’s vertical delta.

var momentumPhase: NSEvent.Phase

The momentum phase for a scroll or flick gesture.

