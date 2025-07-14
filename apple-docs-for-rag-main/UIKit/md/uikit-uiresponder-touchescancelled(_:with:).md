

- UIKit
- UIResponder
-  touchesCancelled(\_:with:) 

Instance Method

# touchesCancelled(\_:with:)

Tells the responder when a system event (such as a system alert) cancels a touch sequence.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func touchesCancelled(
    _ touches: Set,
    with event: UIEvent?
)
```

## Parameters 

`touches`  

A set of UITouch instances that represent the touches for the ending phase of the event represented by `event`. For touches in a view, this set contains only one touch by default. To receive multiple touches, you must set the view’s isMultipleTouchEnabled property to true.

`event`  

The event to which the touches belong.

## Mentioned in 

Implementing a Multi-Touch app

About the Gesture Recognizer State Machine

Implementing a Discrete Gesture Recognizer

Implementing a Continuous Gesture Recognizer

Implementing coalesced touch support in an app

## Discussion

UIKit calls this method when it receives a system interruption requiring cancellation of the touch sequence. An interruption is anything that causes the application to become inactive or causes the view handling the touch events to be removed from its window. Your implementation of this method should clean up any state associated with handling the touch sequence. The default implementation of this method forwards the message up the responder chain. When creating your own subclasses, call `super` to forward any events that you don’t handle yourself, like in the following code.

- Swift
- Objective-C

```
super.touchesCancelled(touches, with: event)
```

```
[super touchesCancelled:touches withEvent:event];
```

If you override this method without calling `super` (a common use pattern), you must also override the other methods for handling touch events, if only as stub (empty) implementations.

## See Also

### Responding to touch events

func touchesBegan(Set&lt;UITouch>, with: UIEvent?)

Tells this object that one or more new touches occurred in a view or window.

func touchesMoved(Set&lt;UITouch>, with: UIEvent?)

Tells the responder when one or more touches associated with an event changed.

func touchesEnded(Set&lt;UITouch>, with: UIEvent?)

Tells the responder when one or more fingers are raised from a view or window.

func touchesEstimatedPropertiesUpdated(Set&lt;UITouch>)

Tells the responder that updated values were received for previously estimated properties or that an update is no longer expected.

