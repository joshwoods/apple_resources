

- AppKit
- NSGestureRecognizer
-  canBePrevented(by:) 

Instance Method

# canBePrevented(by:)

Overridden to indicate that the specified gesture recognizer can prevent the current object from recognizing a gesture.

macOS

``` source
@MainActor
func canBePrevented(by preventingGestureRecognizer: NSGestureRecognizer) -> Bool
```

## Parameters 

`preventingGestureRecognizer`  

The gesture recognizer that can prevent the current object from recognizing its gesture.

## Return Value

true to indicate that `preventingGestureRecognizer` can block the current gesture recognizer from recognizing its gesture, or false if both gesture recognizers can operate simultaneously.

## Discussion

This method enables similar behavior as the gestureRecognizerShouldBegin(_:) and gestureRecognizer(_:shouldRequireFailureOf:) methods of the gesture recognizer’s delegate. Using this method lets you define rules that apply to all instances of your custom gesture recognizer class. For example, a gesture recognizer of a given class might want to prevent instances of the same class from recognizing at the same time.

## See Also

### Methods for Subclasses

func reset()

Overridden to reset the internal state of the gesture recognizer when an attempt completes.

func mouseDown(with: NSEvent)

Informs the gesture recognizer that the user pressed the left mouse button.

func mouseDragged(with: NSEvent)

Informs the gesture recognizer that the user moved the mouse with the left button pressed.

func mouseUp(with: NSEvent)

Informs the gesture recognizer that the user released the left mouse button.

func otherMouseDown(with: NSEvent)

Informs the gesture recognizer that the user pressed a mouse button other than the left or right one.

func otherMouseDragged(with: NSEvent)

Informs the gesture recognizer that the user moved the mouse with a button other than the left or right one pressed.

func otherMouseUp(with: NSEvent)

Informs the gesture recognizer that the user released a mouse button other than the left or right one.

func rightMouseDown(with: NSEvent)

Informs the gesture recognizer that the user pressed the right mouse button.

func rightMouseDragged(with: NSEvent)

Informs the gesture recognizer that the user moved the mouse with the right button pressed.

func rightMouseUp(with: NSEvent)

Informs the gesture recognizer that the user released the right mouse button.

func magnify(with: NSEvent)

Informs the gesture recognizer that the user is performing a pinch gesture.

func rotate(with: NSEvent)

Informs the gesture recognizer that the user is performing a rotation gesture.

func canPrevent(NSGestureRecognizer) -> Bool

Overridden to indicate that the current object can prevent the specified gesture recognizer from recognizing its gesture.

func shouldBeRequiredToFail(by: NSGestureRecognizer) -> Bool

Overridden to indicate that the current object must fail before the specified gesture recognizer begins recognizing its gesture.

func shouldRequireFailure(of: NSGestureRecognizer) -> Bool

Overridden to indicate that the specified gesture recognizer must fail before the current object begins recognizing its gesture.

