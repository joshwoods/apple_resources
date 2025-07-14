

- Quartz
- QCView
-  openGLContext() Deprecated

Instance Method

# openGLContext()

Returns the OpenGL context used by the view.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func openGLContext() -> NSOpenGLContext!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

An `NSOpenGLContext` object.

## Discussion

This context as a read-only object . Do not attempt to change any of its settings. If you subclass `QCView` so that you can perform custom OpenGL drawing, you’ll need to use this method to retrieve the view’s OpenGL context.

## See Also

### Related Documentation

func render(atTime: TimeInterval, arguments: [AnyHashable : Any]!) -> Bool

Overrides to perform your custom operations prior to or after rendering a frame of a composition.

Deprecated

### Working With OpenGL

func openGLPixelFormat() -> NSOpenGLPixelFormat!

Returns the OpenGL pixel format used by the view.

Deprecated

