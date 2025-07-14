

- AppKit
- NSOpenGLContext
-  clearDrawable() Deprecated

Instance Method

# clearDrawable()

Disassociates the OpenGL context from its viewport.

macOS 10.0–10.14Deprecated

``` source
func clearDrawable()
```

Deprecated

Please use Metal or MetalKit.

## Discussion

This method disassociates the receiver from any associated `NSView` object. If the receiver is in full-screen or offscreen mode, it exits that mode.

## See Also

### Managing the Drawable Object

var view: NSView?

Returns the OpenGL context’s view.

Deprecated

func update()

Updates the OpenGL context’s drawable object.

Deprecated

