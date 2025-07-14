

- AppKit
- NSOpenGLContext
-  flushBuffer() Deprecated

Instance Method

# flushBuffer()

Copies the back buffer to the front buffer of the OpenGL context.

macOS 10.0–10.14Deprecated

``` source
func flushBuffer()
```

Deprecated

Please use Metal or MetalKit.

## Discussion

If the receiver is not a double-buffered context, this call does nothing.

If the NSOpenGLPixelFormat object used to create the context had a false backing store attribute (`NSOpenGLPFABackingStore`), the buffers may be exchanged rather than copied. This is often the case in full-screen mode.

According to the swap interval context attribute (see NSOpenGLCPSwapInterval), the copy may take place during the vertical retrace of the monitor, rather than immediately after flushBuffer() is called. An implicit `glFlush` is done by flushBuffer() before it returns. For optimal performance, an application should not call `glFlush` immediately before calling flushBuffer(). Subsequent OpenGL commands can be issued immediately after calling flushBuffer(), but are not executed until the buffer copy is completed.

## See Also

### Related Documentation

func getValues(UnsafeMutablePointer&lt;GLint>, for: NSOpenGLContext.Parameter)

Returns the value of the requested parameter.

Deprecated

init?(format: NSOpenGLPixelFormat, share: NSOpenGLContext?)

Returns an OpenGL context object initialized with the specified pixel format information.

Deprecated

func setValues(UnsafePointer&lt;GLint>, for: NSOpenGLContext.Parameter)

Sets the value of the specified parameter.

Deprecated

