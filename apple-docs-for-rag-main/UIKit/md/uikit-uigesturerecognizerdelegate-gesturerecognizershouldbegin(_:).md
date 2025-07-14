

- UIKit
- UIGestureRecognizerDelegate
-  gestureRecognizerShouldBegin(\_:) 

Instance Method

# gestureRecognizerShouldBegin(\_:)

Asks the delegate if a gesture recognizer should begin interpreting touches.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func gestureRecognizerShouldBegin(_ gestureRecognizer: UIGestureRecognizer) -> Bool
```

## Parameters 

`gestureRecognizer`  

An instance of a subclass of the abstract base class UIGestureRecognizer. This gesture-recognizer object is about to begin processing touches to determine if its gesture is occurring.

## Return Value

true (the default) to tell the gesture recognizer to proceed with interpreting touches, false to prevent it from attempting to recognize its gesture.

## Discussion

This method is called when a gesture recognizer attempts to transition out of the UIGestureRecognizer.State.possible state. Returning false causes the gesture recognizer to transition to the UIGestureRecognizer.State.failed state.

## See Also

### Regulating gesture recognition

func gestureRecognizer(UIGestureRecognizer, shouldReceive: UITouch) -> Bool

Asks the delegate if a gesture recognizer should receive an object representing a touch.

func gestureRecognizer(UIGestureRecognizer, shouldReceive: UIPress) -> Bool

Asks the delegate if a gesture recognizer should receive an object representing a press.

func gestureRecognizer(UIGestureRecognizer, shouldReceive: UIEvent) -> Bool

Asks the delegate if a gesture recognizer should receive an object representing a touch or press event.

