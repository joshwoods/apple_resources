

- RealityKit
- ARView
-  mouseDragged(with:) 

Instance Method

# mouseDragged(with:)

Informs the view that the user has moved the mouse with the left button pressed.

macOS

``` source
@MainActor @preconcurrency
override dynamic func mouseDragged(with event: NSEvent)
```

## Parameters 

`event`  

An object encapsulating information about the mouse event.

## Discussion

The view handles the event instead of passing it to the next responder. See NSResponder for more information about the responder chain.

## See Also

### Handling mouse input

func mouseDown(with: NSEvent)

Informs the view that the user has pressed the left mouse button.

func mouseUp(with: NSEvent)

Informs the view that the user has released the left mouse button.

func mouseMoved(with: NSEvent)

Informs the view that the mouse has moved.

func rightMouseDown(with: NSEvent)

Informs the view that the user has pressed the right mouse button.

func rightMouseDragged(with: NSEvent)

Informs the view that the user has moved the mouse with the right button pressed.

func rightMouseUp(with: NSEvent)

Informs the view that the user has released the right mouse button.

func otherMouseDown(with: NSEvent)

Informs the view that the user has pressed a mouse button other than the left or right one.

func otherMouseDragged(with: NSEvent)

Informs the view that the user has moved the mouse with a button other than the left or right button pressed.

func otherMouseUp(with: NSEvent)

Informs the view that the user has released a mouse button other than the left or right button.

func scrollWheel(with: NSEvent)

Informs the view that the mouse’s scroll wheel has moved.

