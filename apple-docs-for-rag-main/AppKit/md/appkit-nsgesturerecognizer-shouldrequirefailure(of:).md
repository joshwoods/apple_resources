

- AppKit
- NSGestureRecognizer
-  shouldRequireFailure(of:) 

Instance Method

# shouldRequireFailure(of:)

Overridden to indicate that the specified gesture recognizer must fail before the current object begins recognizing its gesture.

macOS

``` source
@MainActor
func shouldRequireFailure(of otherGestureRecognizer: NSGestureRecognizer) -> Bool
```

## Parameters 

`otherGestureRecognizer`  

The gesture recognizer that must fail before the current object is allowed to recognize its gesture.

## Return Value

true to cause the current object to wait to recognize its own gesture until the object in otherGestureRecognizer fails.

## Discussion

Using this method lets you define rules that apply to all instances of your custom gesture recognizer class.

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

func canBePrevented(by: NSGestureRecognizer) -> Bool

Overridden to indicate that the specified gesture recognizer can prevent the current object from recognizing a gesture.

func canPrevent(NSGestureRecognizer) -> Bool

Overridden to indicate that the current object can prevent the specified gesture recognizer from recognizing its gesture.

func shouldBeRequiredToFail(by: NSGestureRecognizer) -> Bool

Overridden to indicate that the current object must fail before the specified gesture recognizer begins recognizing its gesture.

