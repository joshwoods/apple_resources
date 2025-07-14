

- UIKit
- UIGestureRecognizer
-  touchesMoved(\_:with:) 

Instance Method

# touchesMoved(\_:with:)

Sent to the gesture recognizer when one or more fingers move in the associated view.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func touchesMoved(
    _ touches: Set,
    with event: UIEvent
)
```

## Parameters 

`touches`  

A set of UITouch instances in the event represented by `event` that represent touches in the UITouch.Phase.moved phase.

`event`  

A UIEvent object representing the event to which the touches belong.

## Discussion

This method has the same exact signature as the corresponding one declared by UIResponder. Through this method a gesture recognizer receives touch objects (in their UITouch.Phase.moved phase) before the view attached to the gesture recognizer receives them. `UIGestureRecognizer` objects are not in the responder chain, yet observe touches hit-tested to their view and their view’s subviews. After observation, the delivery of touch objects to the attached view, or their disposition otherwise, is affected by the cancelsTouchesInView, delaysTouchesBegan, and delaysTouchesEnded properties.

If the gesture recognizer is interpreting a continuous gesture, it should set its state to UIGestureRecognizer.State.changed upon receiving this message. If at any point in its handling of the touch objects the gesture recognizer determines that the multi-touch event sequence is not its gesture, it should set it state to UIGestureRecognizer.State.cancelled .

Multiple touches are disabled by default. In order to receive multiple touch events you must set the a isMultipleTouchEnabled property of the attached view instance to true.

## See Also

### Implementing subclasses

func touchesBegan(Set&lt;UITouch>, with: UIEvent)

Sent to the gesture recognizer when one or more fingers touch down in the associated view.

func touchesEnded(Set&lt;UITouch>, with: UIEvent)

Sent to the gesture recognizer when one or more fingers lift from the associated view.

func touchesCancelled(Set&lt;UITouch>, with: UIEvent)

Sent to the gesture recognizer when a system event (such as an incoming phone call) cancels a touch event.

func touchesEstimatedPropertiesUpdated(Set&lt;UITouch>)

Sent to the gesture recognizer when the estimated properties for a touch have changed so that they are no longer estimated, or an update is no longer expected.

func reset()

Overridden to reset internal state when a gesture recognition attempt completes.

func ignore(UITouch, for: UIEvent)

Tells the gesture recognizer to ignore a specific touch of the given event.

func canBePrevented(by: UIGestureRecognizer) -> Bool

Overridden to indicate that the specified gesture recognizer can prevent the receiver from recognizing a gesture.

func canPrevent(UIGestureRecognizer) -> Bool

Overridden to indicate that the receiver can prevent the specified gesture recognizer from recognizing its gesture.

func shouldReceive(UIEvent) -> Bool

func shouldRequireFailure(of: UIGestureRecognizer) -> Bool

Overridden to indicate that the receiver requires the specified gesture recognizer to fail.

func shouldBeRequiredToFail(by: UIGestureRecognizer) -> Bool

Overridden to indicate that the receiver should be required to fail by the specified gesture recognizer.

func ignore(UIPress, for: UIPressesEvent)

Tells the gesture recognizer to ignore a specific press of the given event.

func pressesBegan(Set&lt;UIPress>, with: UIPressesEvent)

Sent to the receiver when a physical button is pressed in the associated view.

func pressesChanged(Set&lt;UIPress>, with: UIPressesEvent)

Sent to the receiver when the force of the press has changed in the associated view.

func pressesEnded(Set&lt;UIPress>, with: UIPressesEvent)

Sent to the receiver when a button is released from the associated view.

