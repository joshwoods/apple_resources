

- AppKit
- NSOpenGLContext
-  update() Deprecated

Instance Method

# update()

Updates the OpenGL context’s drawable object.

macOS 10.0–10.14Deprecated

``` source
@MainActor
func update()
```

Deprecated

Please use Metal or MetalKit.

## Discussion

Call this method whenever the receiver’s drawable object changes size or location. A multithreaded application must synchronize all threads that access the same drawable object and call update() for each thread’s context serially.

## See Also

### Managing the Drawable Object

var view: NSView?

Returns the OpenGL context’s view.

Deprecated

func clearDrawable()

Disassociates the OpenGL context from its viewport.

Deprecated

