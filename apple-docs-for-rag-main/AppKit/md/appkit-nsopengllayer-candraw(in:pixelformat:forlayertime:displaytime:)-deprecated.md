

- AppKit
- NSOpenGLLayer
-  canDraw(in:pixelFormat:forLayerTime:displayTime:) Deprecated

Instance Method

# canDraw(in:pixelFormat:forLayerTime:displayTime:)

Invoked to ask the layer whether it can (or should) draw.

macOS 10.6–10.14Deprecated

``` source
func canDraw(
    in context: NSOpenGLContext,
    pixelFormat: NSOpenGLPixelFormat,
    forLayerTime t: CFTimeInterval,
    displayTime ts: UnsafePointer
) -> Bool
```

Deprecated

Please use CAMetalLayer instead.

## Parameters 

`context`  

The NSOpenGLContext in to which the OpenGL content would be drawn.

`pixelFormat`  

The pixel format used when the context was created.

`t`  

The current layer time.

`ts`  

The display timestamp associated with timeInterval. Can be `null`.

## Return Value

true if the receiver should render OpenGL content, false otherwise.

## Discussion

This method is called before attempting to render the frame for the layer time specified by `timeInterval`. If the method returns false, the frame is skipped. The default implementation always returns true.

## See Also

### Related Documentation

Core Animation Programming Guide

### Drawing the Content

func draw(in: NSOpenGLContext, pixelFormat: NSOpenGLPixelFormat, forLayerTime: CFTimeInterval, displayTime: UnsafePointer&lt;CVTimeStamp>)

Draws the OpenGL content for the specified time.

Deprecated

