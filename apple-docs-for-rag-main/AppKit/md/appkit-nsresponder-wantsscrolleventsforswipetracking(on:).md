

- AppKit
- NSResponder
-  wantsScrollEventsForSwipeTracking(on:) 

Instance Method

# wantsScrollEventsForSwipeTracking(on:)

Implement this method to track gesture scroll events such as a swipe.

macOS 10.7+

``` source
@MainActor
func wantsScrollEventsForSwipeTracking(on axis: NSEvent.GestureAxis) -> Bool
```

## Parameters 

`axis`  

The event gesture axis of the swipe, which defines the scroll direction.

## Return Value

true if gesture scroll events are to be forwarded up the responder chain; otherwise false. The default implementation returns false.

## Discussion

Implement this method in your swipe controller and return true to inform views that perform elastic scrolling to forward gesture scroll events up the responder chain. The events are forwarded only on the following condition: the content to be scrolled is already at the edge of the scrolled direction when the scroll gesture begins. Otherwise, the view performs elastic scrolling. The default implementation returns false.

## See Also

### Related Documentation

func trackSwipeEvent(options: NSEvent.SwipeTrackingOptions, dampenAmountThresholdMin: CGFloat, max: CGFloat, usingHandler: (CGFloat, NSEvent.Phase, Bool, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Allows tracking and user interface feedback of scroll wheel events.

### Touch and Gesture Events

func beginGesture(with: NSEvent)

Informs the receiver that the user has begun a touch gesture.

func endGesture(with: NSEvent)

Informs the receiver that the user has ended a touch gesture.

func magnify(with: NSEvent)

Informs the receiver that the user has begun a pinch gesture.

func rotate(with: NSEvent)

Informs the receiver that the user has begun a rotation gesture.

func swipe(with: NSEvent)

Informs the receiver that the user has begun a swipe gesture.

func touchesBegan(with: NSEvent)

Informs the receiver that new set of touches has been recognized.

func touchesMoved(with: NSEvent)

Informs the receiver that one or more touches has moved.

func touchesCancelled(with: NSEvent)

Informs the receiver that tracking of touches has been cancelled for any reason.

func touchesEnded(with: NSEvent)

Returns that a set of touches have been removed.

func wantsForwardedScrollEvents(for: NSEvent.GestureAxis) -> Bool

Returns whether to forward elastic scrolling gesture events up the responder.

func smartMagnify(with: NSEvent)

Informs the receiver that the user performed a smart zoom gesture.

enum GestureAxis

Constants that specify the direction of travel for a gesture.

