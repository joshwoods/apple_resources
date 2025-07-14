

- AppKit
- NSOpenGLContext
-  view Deprecated

Instance Property

# view

Returns the OpenGL context’s view.

macOS 10.0–10.14Deprecated

``` source
@MainActor
weak var view: NSView? { get set }
```

## Return Value

The view, or `nil` if the receiver has no drawable object, is in full-screen mode, or is in offscreen mode.

## See Also

### Managing the Drawable Object

func clearDrawable()

Disassociates the OpenGL context from its viewport.

Deprecated

func update()

Updates the OpenGL context’s drawable object.

Deprecated

