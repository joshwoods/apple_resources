

- AppKit
- NSGestureRecognizer
-  mouseDragged(with:) 

Instance Method

# mouseDragged(with:)

Informs the gesture recognizer that the user moved the mouse with the left button pressed.

macOS

``` source
@MainActor
func mouseDragged(with event: NSEvent)
```

## Parameters 

`event`  

An object encapsulating information about the mouse-dragged event.

## Discussion

The default implementation of this method does nothing. Use this method to update the state of your gesture recognizer in whatever way is appropriate.

A gesture recognizer monitors events that occur in its view (and any subviews) but does not take part in the responder chain itself. The gesture recognizer receives events before any views do. Use the delaysPrimaryMouseButtonEvents property to control whether `event` is propagated to the view.

## See Also

### Methods for Subclasses

func reset()

Overridden to reset the internal state of the gesture recognizer when an attempt completes.

func mouseDown(with: NSEvent)

Informs the gesture recognizer that the user pressed the left mouse button.

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

func shouldRequireFailure(of: NSGestureRecognizer) -> Bool

Overridden to indicate that the specified gesture recognizer must fail before the current object begins recognizing its gesture.

