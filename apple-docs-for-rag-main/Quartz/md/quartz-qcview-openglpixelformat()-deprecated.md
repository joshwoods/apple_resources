

- Quartz
- QCView
-  openGLPixelFormat() Deprecated

Instance Method

# openGLPixelFormat()

Returns the OpenGL pixel format used by the view.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func openGLPixelFormat() -> NSOpenGLPixelFormat!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

An `NSOpenGLPixelFormat` object.

## Discussion

This pixel format as a read-only object. Do not attempt to change any of its settings.

## See Also

### Working With OpenGL

func openGLContext() -> NSOpenGLContext!

Returns the OpenGL context used by the view.

Deprecated

