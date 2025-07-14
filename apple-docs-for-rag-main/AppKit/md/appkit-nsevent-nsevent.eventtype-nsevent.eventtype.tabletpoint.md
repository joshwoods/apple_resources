

- AppKit
- NSEvent
- NSEvent.EventType
-  NSEvent.EventType.tabletPoint 

Case

# NSEvent.EventType.tabletPoint

The user touched a point on a tablet.

macOS

``` source
case tabletPoint
```

## Discussion

Tablets generate tablet-point events between a mouse-down event and the first mouse drag event.

## See Also

### Getting Touch-Based Events

case beginGesture

An event marking the beginning of a gesture.

case endGesture

An event that marks the end of a gesture.

case magnify

The user performed a pinch-open or pinch-close gesture.

case smartMagnify

The user performed a smart-zoom gesture.

case swipe

The user performed a swipe gesture.

case rotate

The user performed a rotate gesture.

case gesture

The user performed a nonspecific type of gesture.

case directTouch

The user touched a portion of the touch bar.

case tabletProximity

A pointing device is near, but not touching, the associated tablet.

case pressure

An event that reports a change in pressure on a pressure-sensitive device.

