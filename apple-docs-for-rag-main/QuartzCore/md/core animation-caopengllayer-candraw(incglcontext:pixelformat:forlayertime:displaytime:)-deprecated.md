

- Core Animation
- CAOpenGLLayer
-  canDraw(inCGLContext:pixelFormat:forLayerTime:displayTime:) Deprecated

Instance Method

# canDraw(inCGLContext:pixelFormat:forLayerTime:displayTime:)

Returns whether the receiver should draw OpenGL content for the specified time.

Mac Catalyst 13.1–13.1DeprecatedmacOS 10.5–10.14Deprecated

``` source
func canDraw(
    inCGLContext ctx: CGLContextObj,
    pixelFormat pf: CGLPixelFormatObj,
    forLayerTime t: CFTimeInterval,
    displayTime ts: UnsafePointer?
) -> Bool
```

Deprecated

OpenGL is deprecated

## Parameters 

`ctx`  

The `CGLContextObj` in to which the OpenGL content would be drawn.

`pf`  

The pixel format used when the `glContext` was created.

`t`  

The current layer time.

`ts`  

The display timestamp associated with `timeInterval`. Can be `null`.

## Return Value

true if the receiver should render OpenGL content, false otherwise.

## Discussion

This method is called before attempting to render the frame for the layer time specified by `timeInterval`. If the method returns false, the frame is skipped. The default implementation always returns true.

## See Also

### Drawing Layer Content

var isAsynchronous: Bool

Determines when the contents of the layer are updated.

Deprecated

func draw(inCGLContext: CGLContextObj, pixelFormat: CGLPixelFormatObj, forLayerTime: CFTimeInterval, displayTime: UnsafePointer&lt;CVTimeStamp>?)

Draws the OpenGL content for the specified time.

Deprecated

