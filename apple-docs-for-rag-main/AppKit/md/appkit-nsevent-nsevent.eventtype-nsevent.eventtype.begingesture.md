

- AppKit
- NSEvent
- NSEvent.EventType
-  NSEvent.EventType.beginGesture 

Case

# NSEvent.EventType.beginGesture

An event marking the beginning of a gesture.

macOS 10.5+

``` source
case beginGesture
```

## Discussion

Note that apps that link against macOS 10.11 and later no longer receive this event type. If you need to access the phases of a specific gesture, you can implement the responder for that gesture and examine its phase property instead.

## See Also

### Getting Touch-Based Events

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

case tabletPoint

The user touched a point on a tablet.

case tabletProximity

A pointing device is near, but not touching, the associated tablet.

case pressure

An event that reports a change in pressure on a pressure-sensitive device.

