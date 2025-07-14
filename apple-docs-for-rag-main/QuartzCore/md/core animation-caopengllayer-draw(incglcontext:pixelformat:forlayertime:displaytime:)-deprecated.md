

- Core Animation
- CAOpenGLLayer
-  draw(inCGLContext:pixelFormat:forLayerTime:displayTime:) Deprecated

Instance Method

# draw(inCGLContext:pixelFormat:forLayerTime:displayTime:)

Draws the OpenGL content for the specified time.

Mac Catalyst 13.1–13.1DeprecatedmacOS 10.5–10.14Deprecated

``` source
func draw(
    inCGLContext ctx: CGLContextObj,
    pixelFormat pf: CGLPixelFormatObj,
    forLayerTime t: CFTimeInterval,
    displayTime ts: UnsafePointer?
)
```

Deprecated

OpenGL is deprecated

## Parameters 

`ctx`  

The rendering context in to which the OpenGL content should be rendered.

`pf`  

The pixel format used when the `glContext` was created.

`t`  

The current layer time.

`ts`  

The display timestamp associated with `timeInterval`. Can be `null`.

## Discussion

This method is called when a new frame needs to be generated for the layer time specified by `timeInterval`. The viewport of `glContext` is set correctly for the size of the layer. No other state is defined. If the method enables OpenGL features, it should disable them before returning.

The default implementation of the method flushes the context.

## See Also

### Drawing Layer Content

var isAsynchronous: Bool

Determines when the contents of the layer are updated.

Deprecated

func canDraw(inCGLContext: CGLContextObj, pixelFormat: CGLPixelFormatObj, forLayerTime: CFTimeInterval, displayTime: UnsafePointer&lt;CVTimeStamp>?) -> Bool

Returns whether the receiver should draw OpenGL content for the specified time.

Deprecated

