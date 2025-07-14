

- AppKit
- NSGestureRecognizer
-  pressureChange(with:) 

Instance Method

# pressureChange(with:)

Informs the current object that a pressure change occurred on a system that supports pressure sensitivity.

macOS 10.10.3+

``` source
@MainActor
func pressureChange(with event: NSEvent)
```

## Parameters 

`event`  

An `NSEvent` object encapsulating information about the event that invoked the change in pressure.

## Discussion

This method is invoked automatically in response to user actions. `event` is the event that initiated the change in pressure.

The default implementation of this method does nothing. Use this method to update the state of your gesture recognizer in whatever way is appropriate.

A gesture recognizer monitors events that occur in its view (and any subviews) but does not take part in the responder chain itself. The gesture recognizer receives events before any views do.

## See Also

### Related Documentation

class NSEvent

An object that contains information about an input action, such as a mouse click or a key press.

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

