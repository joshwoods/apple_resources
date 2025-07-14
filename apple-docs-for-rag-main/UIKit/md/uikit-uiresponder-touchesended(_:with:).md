

- UIKit
- UIResponder
-  touchesEnded(\_:with:) 

Instance Method

# touchesEnded(\_:with:)

Tells the responder when one or more fingers are raised from a view or window.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func touchesEnded(
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

Implementing coalesced touch support in an app

Implementing a Discrete Gesture Recognizer

Implementing a Continuous Gesture Recognizer

## Discussion

UIKit calls this method when a finger or Apple Pencil is no longer touching the screen. Many UIKit classes override this method and use it to clean up state involved in the handling of the corresponding touch events. The default implementation of this method forwards the message up the responder chain. When creating your own subclasses, call `super` to forward any events that you don’t handle yourself, like in the following code.

- Swift
- Objective-C

```
super.touchesEnded(touches, with: event)
```

```
[super touchesEnded:touches withEvent:event];
```

If you override this method without calling super (a common use pattern), you must also override the other methods for handling touch events, even if your implementations do nothing.

Note

In iOS 17, Messages allows you to interactively resize iMessage apps with a vertical pan gesture. Messages handles any conflicts between resize gestures and your custom gestures. If your app uses manual touch handling, override those methods in your app’s UIView. You can either change your manual touch handling code to use a gesture recognizer instead, or your UIView can override gestureRecognizerShouldBegin(_:) and return NO when your iMessage app doesn’t own the gesture.

## See Also

### Responding to touch events

func touchesBegan(Set&lt;UITouch>, with: UIEvent?)

Tells this object that one or more new touches occurred in a view or window.

func touchesMoved(Set&lt;UITouch>, with: UIEvent?)

Tells the responder when one or more touches associated with an event changed.

func touchesCancelled(Set&lt;UITouch>, with: UIEvent?)

Tells the responder when a system event (such as a system alert) cancels a touch sequence.

func touchesEstimatedPropertiesUpdated(Set&lt;UITouch>)

Tells the responder that updated values were received for previously estimated properties or that an update is no longer expected.

