

- AppKit
- NSResponder
-  rightMouseDown(with:) 

Instance Method

# rightMouseDown(with:)

Informs the receiver that the user has pressed the right mouse button.

macOS

``` source
@MainActor
func rightMouseDown(with event: NSEvent)
```

## Parameters 

`event`  

An object encapsulating information about the mouse-down event.

## Discussion

The default implementation simply passes this message to the next responder.

Note

Prior to OS X v10.7, NSView did not pass unhandled rightMouseDown(with:) events up the responder chain. In macOS 10.7 and later, NSView passes rightMouseDown(with:) events up the responder chain if AppKit doesn’t find an associated context menu to display for the view. To avoid binary compatibility issues, this new behavior is enabled only for applications linked on macOS 10.7 or later.

## See Also

### Responding to Mouse Events

func mouseDown(with: NSEvent)

Informs the receiver that the user has pressed the left mouse button.

func mouseDragged(with: NSEvent)

Informs the receiver that the user has moved the mouse with the left button pressed.

func mouseUp(with: NSEvent)

Informs the receiver that the user has released the left mouse button.

func mouseMoved(with: NSEvent)

Informs the receiver that the mouse has moved.

func mouseEntered(with: NSEvent)

Informs the receiver that the cursor has entered a tracking rectangle.

func mouseExited(with: NSEvent)

Informs the receiver that the cursor has exited a tracking rectangle.

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

