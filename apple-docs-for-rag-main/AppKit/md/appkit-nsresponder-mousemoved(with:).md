

- AppKit
- NSResponder
-  mouseMoved(with:) 

Instance Method

# mouseMoved(with:)

Informs the receiver that the mouse has moved.

macOS

``` source
@MainActor
func mouseMoved(with event: NSEvent)
```

## Parameters 

`event`  

An object encapsulating information about the mouse-moved event.

## Discussion

The default implementation simply passes this message to the next responder.

## See Also

### Related Documentation

var acceptsMouseMovedEvents: Bool

A Boolean value that indicates whether the window accepts mouse-moved events.

### Responding to Mouse Events

func mouseDown(with: NSEvent)

Informs the receiver that the user has pressed the left mouse button.

func mouseDragged(with: NSEvent)

Informs the receiver that the user has moved the mouse with the left button pressed.

func mouseUp(with: NSEvent)

Informs the receiver that the user has released the left mouse button.

func mouseEntered(with: NSEvent)

Informs the receiver that the cursor has entered a tracking rectangle.

func mouseExited(with: NSEvent)

Informs the receiver that the cursor has exited a tracking rectangle.

func rightMouseDown(with: NSEvent)

Informs the receiver that the user has pressed the right mouse button.

func rightMouseDragged(with: NSEvent)

Informs the receiver that the user has moved the mouse with the right button pressed.

func rightMouseUp(with: NSEvent)

Informs the receiver that the user has released the right mouse button.

func otherMouseDown(with: NSEvent)

Informs the receiver that the user has pressed a mouse button other than the left or right one.

func otherMouseDragged(with: NSEvent)

Informs the receiver that the user has moved the mouse with a button other than the left or right button pressed.

func otherMouseUp(with: NSEvent)

Informs the receiver that the user has released a mouse button other than the left or right button.

