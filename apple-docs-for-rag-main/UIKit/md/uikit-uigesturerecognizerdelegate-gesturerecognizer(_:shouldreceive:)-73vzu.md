

- UIKit
- UIGestureRecognizerDelegate
-  gestureRecognizer(\_:shouldReceive:) 

Instance Method

# gestureRecognizer(\_:shouldReceive:)

Asks the delegate if a gesture recognizer should receive an object representing a press.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func gestureRecognizer(
    _ gestureRecognizer: UIGestureRecognizer,
    shouldReceive press: UIPress
) -> Bool
```

## Parameters 

`gestureRecognizer`  

An instance of a subclass of the abstract base class UIGestureRecognizer.

`press`  

A UIPress object from the current press sequence.

## Return Value

true (the default) to allow the gesture recognizer to examine the press object, or false to prevent the gesture recognizer from seeing this press object.

## Discussion

UIKit calls this method before the pressesBegan(_:with:) method of the gesture recognizer.

## See Also

### Regulating gesture recognition

func gestureRecognizerShouldBegin(UIGestureRecognizer) -> Bool

Asks the delegate if a gesture recognizer should begin interpreting touches.

func gestureRecognizer(UIGestureRecognizer, shouldReceive: UITouch) -> Bool

Asks the delegate if a gesture recognizer should receive an object representing a touch.

func gestureRecognizer(UIGestureRecognizer, shouldReceive: UIEvent) -> Bool

Asks the delegate if a gesture recognizer should receive an object representing a touch or press event.

