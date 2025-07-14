

- AppKit
- NSResponder
-  touchesBegan(with:) 

Instance Method

# touchesBegan(with:)

Informs the receiver that new set of touches has been recognized.

macOS 10.6+

``` source
@MainActor
func touchesBegan(with event: NSEvent)
```

## Parameters 

`event`  

An event object representing the beginning of a touch.

## Discussion

The system sends the event to the view under the touch in the key window. To get the set of touches that began for this view (or descendants of this view) call touches(matching:in:) on `event` and pass began for the phase send.

This isn’t always the point of contact with the touch device. A touch that transitions from resting to active may be part of a touchesBegan(with:) set.

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

func wantsScrollEventsForSwipeTracking(on: NSEvent.GestureAxis) -> Bool

Implement this method to track gesture scroll events such as a swipe.

enum GestureAxis

Constants that specify the direction of travel for a gesture.

