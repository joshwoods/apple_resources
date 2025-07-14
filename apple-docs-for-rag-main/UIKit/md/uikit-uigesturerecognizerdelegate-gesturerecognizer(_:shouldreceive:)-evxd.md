

- UIKit
- UIGestureRecognizerDelegate
-  gestureRecognizer(\_:shouldReceive:) 

Instance Method

# gestureRecognizer(\_:shouldReceive:)

Asks the delegate if a gesture recognizer should receive an object representing a touch or press event.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+tvOS 13.4+visionOS 1.0+

``` source
@MainActor
optional func gestureRecognizer(
    _ gestureRecognizer: UIGestureRecognizer,
    shouldReceive event: UIEvent
) -> Bool
```

## Parameters 

`gestureRecognizer`  

An instance of a subclass of the abstract base class UIGestureRecognizer.

`event`  

A UIEvent object from the current press or touch sequence.

## Return Value

Return false to prevent the gesture recognizer from seeing this event.

## Discussion

UIKit calls this method once before either the gestureRecognizer(_:shouldReceive:) method or the gestureRecognizer(_:shouldReceive:) method of the gesture recognizer.

## See Also

### Regulating gesture recognition

func gestureRecognizerShouldBegin(UIGestureRecognizer) -> Bool

Asks the delegate if a gesture recognizer should begin interpreting touches.

func gestureRecognizer(UIGestureRecognizer, shouldReceive: UITouch) -> Bool

Asks the delegate if a gesture recognizer should receive an object representing a touch.

func gestureRecognizer(UIGestureRecognizer, shouldReceive: UIPress) -> Bool

Asks the delegate if a gesture recognizer should receive an object representing a press.

