

- UIKit
- UIGestureRecognizer
-  touchesEstimatedPropertiesUpdated(\_:) 

Instance Method

# touchesEstimatedPropertiesUpdated(\_:)

Sent to the gesture recognizer when the estimated properties for a touch have changed so that they are no longer estimated, or an update is no longer expected.

iOS 9.1+iPadOS 9.1+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
func touchesEstimatedPropertiesUpdated(_ touches: Set)
```

## Parameters 

`touches`  

The array of UITouch objects containing updated properties.

## Discussion

The default implementation of this method does nothing. Subclasses may override it and use it to process updates to touches.

UIKit calls this method to report updates to properties that were previously declared to be estimates through touchesBegan(_:with:), touchesMoved(_:with:) or touchesEnded(_:with:), and where declared to expect updates by having at least one property set in estimatedPropertiesExpectingUpdates.

Use the estimationUpdateIndex property to correlate the previous state of the touch with the updated state incoming in this method. The updated values are denoted by having a cleared state in the estimatedPropertiesExpectingUpdates bit mask. Although most properties end up with a cleared estimatedProperties flag, a property can stay in the estimated state because of hardware considerations. This behavior allows the client to decide to replace the estimate with a more domain-specific estimate, based on the other touches it receives.

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

