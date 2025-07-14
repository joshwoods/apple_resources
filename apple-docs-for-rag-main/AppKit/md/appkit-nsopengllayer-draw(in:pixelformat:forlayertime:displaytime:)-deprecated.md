

- AppKit
- NSOpenGLLayer
-  draw(in:pixelFormat:forLayerTime:displayTime:) Deprecated

Instance Method

# draw(in:pixelFormat:forLayerTime:displayTime:)

Draws the OpenGL content for the specified time.

macOS 10.6–10.14Deprecated

``` source
func draw(
    in context: NSOpenGLContext,
    pixelFormat: NSOpenGLPixelFormat,
    forLayerTime t: CFTimeInterval,
    displayTime ts: UnsafePointer
)
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

## Discussion

This method is called when a new frame needs to be generated for the layer time specified by timeInterval.

## See Also

### Drawing the Content

func canDraw(in: NSOpenGLContext, pixelFormat: NSOpenGLPixelFormat, forLayerTime: CFTimeInterval, displayTime: UnsafePointer&lt;CVTimeStamp>) -> Bool

Invoked to ask the layer whether it can (or should) draw.

Deprecated

