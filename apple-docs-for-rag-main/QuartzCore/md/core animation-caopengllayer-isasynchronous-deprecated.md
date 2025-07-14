

- Core Animation
- CAOpenGLLayer
-  isAsynchronous Deprecated

Instance Property

# isAsynchronous

Determines when the contents of the layer are updated.

Mac Catalyst 13.1–13.1DeprecatedmacOS 10.5–10.14Deprecated

``` source
var isAsynchronous: Bool { get set }
```

Deprecated

OpenGL is deprecated

## Discussion

If false, the contents of the layer are updated only in response to receiving a setNeedsDisplay() message. When true, the receiver’s canDraw(inCGLContext:pixelFormat:forLayerTime:displayTime:) is called periodically to determine if the OpenGL content should be updated.

## See Also

### Related Documentation

Core Animation Programming Guide

### Drawing Layer Content

func canDraw(inCGLContext: CGLContextObj, pixelFormat: CGLPixelFormatObj, forLayerTime: CFTimeInterval, displayTime: UnsafePointer&lt;CVTimeStamp>?) -> Bool

Returns whether the receiver should draw OpenGL content for the specified time.

Deprecated

func draw(inCGLContext: CGLContextObj, pixelFormat: CGLPixelFormatObj, forLayerTime: CFTimeInterval, displayTime: UnsafePointer&lt;CVTimeStamp>?)

Draws the OpenGL content for the specified time.

Deprecated

