

- UIKit
- UIGestureRecognizer
-  canPrevent(\_:) 

Instance Method

# canPrevent(\_:)

Overridden to indicate that the receiver can prevent the specified gesture recognizer from recognizing its gesture.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func canPrevent(_ preventedGestureRecognizer: UIGestureRecognizer) -> Bool
```

## Parameters 

`preventedGestureRecognizer`  

An instance of a subclass of `UIGestureRecognizer`.

## Return Value

true to indicate that the receiver can block `preventedGestureRecognizer` from recognizing its gesture, otherwise false.

## Discussion

Overriding these methods enables the same behavior as implementing the UIGestureRecognizerDelegate methods gestureRecognizerShouldBegin(_:) and gestureRecognizer(_:shouldReceive:). However, by overriding them, subclasses can define class-wide prevention rules. For example, a UITapGestureRecognizer object never prevents another `UITapGestureRecognizer` object with a higher tap count.

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

