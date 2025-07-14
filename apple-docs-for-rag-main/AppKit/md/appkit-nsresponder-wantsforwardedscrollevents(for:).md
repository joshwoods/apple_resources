

- AppKit
- NSResponder
-  wantsForwardedScrollEvents(for:) 

Instance Method

# wantsForwardedScrollEvents(for:)

Returns whether to forward elastic scrolling gesture events up the responder.

macOS 10.7+

``` source
@MainActor
func wantsForwardedScrollEvents(for axis: NSEvent.GestureAxis) -> Bool
```

## Parameters 

`axis`  

The gesture axis. See NSEvent.GestureAxis for the possible values.

## Return Value

Returns true when forward gesture scroll events should be forwarded up the responder chain when the scrolling content is already at the edge of the scrolled direction at the beginning of the scroll gesture; false otherwise.

## Discussion

Some views process gesture scroll events to perform elastic scrolling. In some cases, you may want to track gesture scroll events like a swipe, see trackSwipeEvent(options:dampenAmountThresholdMin:max:usingHandler:).

Implement this method and return true in your swipe controller and views that perform elastic scrolling will forward gesture scroll events up the responder chain on the following condition: the content to be scrolled is already at the edge of the scrolled direction at the beginning of the scroll gesture.

Otherwise, the view will perform elastic scrolling.

## See Also

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

func smartMagnify(with: NSEvent)

Informs the receiver that the user performed a smart zoom gesture.

func wantsScrollEventsForSwipeTracking(on: NSEvent.GestureAxis) -> Bool

Implement this method to track gesture scroll events such as a swipe.

enum GestureAxis

Constants that specify the direction of travel for a gesture.

