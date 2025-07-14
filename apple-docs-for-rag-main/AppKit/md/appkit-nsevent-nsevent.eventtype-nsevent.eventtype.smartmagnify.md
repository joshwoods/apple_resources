

- AppKit
- NSEvent
- NSEvent.EventType
-  NSEvent.EventType.smartMagnify 

Case

# NSEvent.EventType.smartMagnify

The user performed a smart-zoom gesture.

macOS 10.8+

``` source
case smartMagnify
```

## Discussion

NSEvent.EventType.smartMagnify represents the smart zoom gesture (that is, a two-finger double tap on trackpads), along with a corresponding NSResponder method. In response to this event, you should magnify the content appropriately for your app. For example, you might zoom in on a specific paragraph or image.

## See Also

### Getting Touch-Based Events

case beginGesture

An event marking the beginning of a gesture.

case endGesture

An event that marks the end of a gesture.

case magnify

The user performed a pinch-open or pinch-close gesture.

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

