

- UIKit
- UIGestureRecognizerDelegate
-  gestureRecognizer(\_:shouldReceive:) 

Instance Method

# gestureRecognizer(\_:shouldReceive:)

Asks the delegate if a gesture recognizer should receive an object representing a touch.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func gestureRecognizer(
    _ gestureRecognizer: UIGestureRecognizer,
    shouldReceive touch: UITouch
) -> Bool
```

## Parameters 

`gestureRecognizer`  

An instance of a subclass of the abstract base class UIGestureRecognizer.

`touch`  

A UITouch object from the current multi-touch sequence.

## Return Value

true (the default) to allow the gesture recognizer to examine the touch object, false to prevent the gesture recognizer from seeing this touch object.

## Discussion

UIKit calls this method before calling the touchesBegan(_:with:) method of the gesture recognizer.

## See Also

### Regulating gesture recognition

func gestureRecognizerShouldBegin(UIGestureRecognizer) -> Bool

Asks the delegate if a gesture recognizer should begin interpreting touches.

func gestureRecognizer(UIGestureRecognizer, shouldReceive: UIPress) -> Bool

Asks the delegate if a gesture recognizer should receive an object representing a press.

func gestureRecognizer(UIGestureRecognizer, shouldReceive: UIEvent) -> Bool

Asks the delegate if a gesture recognizer should receive an object representing a touch or press event.

