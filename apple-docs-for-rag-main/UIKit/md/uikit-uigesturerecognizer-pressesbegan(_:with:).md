

- UIKit
- UIGestureRecognizer
-  pressesBegan(\_:with:) 

Instance Method

# pressesBegan(\_:with:)

Sent to the receiver when a physical button is pressed in the associated view.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func pressesBegan(
    _ presses: Set,
    with event: UIPressesEvent
)
```

## Parameters 

`presses`  

A set of UIPress instances in the event represented by `event` that represent the touches in the UIPress.Phase.began phase.

`event`  

A UIEvent object that includes a reference to `press`.

## Discussion

This method has the same signature as the corresponding one declared by UIResponder. With this method, a gesture recognizer receives press objects (in their UIPress.Phase.began phase) before the view attached to the gesture recognizer receives them. `UIGestureRecognizer` objects are not in the responder chain, yet they observe presses hit-tested to their view and their view’s subviews.

If the gesture recognizer is interpreting a continuous gesture, it should set its state to UIGestureRecognizer.State.began upon receiving this message. If at any point in its handling of the press objects the gesture recognizer determines that the press event sequence is not its gesture, it should set its state to UIGestureRecognizer.State.cancelled.

## See Also

### Implementing subclasses

func touchesBegan(Set&lt;UITouch>, with: UIEvent)

Sent to the gesture recognizer when one or more fingers touch down in the associated view.

func touchesMoved(Set&lt;UITouch>, with: UIEvent)

Sent to the gesture recognizer when one or more fingers move in the associated view.

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

func pressesChanged(Set&lt;UIPress>, with: UIPressesEvent)

Sent to the receiver when the force of the press has changed in the associated view.

func pressesEnded(Set&lt;UIPress>, with: UIPressesEvent)

Sent to the receiver when a button is released from the associated view.

