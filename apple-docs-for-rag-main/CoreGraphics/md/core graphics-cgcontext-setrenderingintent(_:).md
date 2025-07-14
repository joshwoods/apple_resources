

- Core Graphics
- CGContext
-  setRenderingIntent(\_:) 

Instance Method

# setRenderingIntent(\_:)

Sets the rendering intent in the current graphics state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setRenderingIntent(_ intent: CGColorRenderingIntent)
```

## Parameters 

`intent`  

A rendering intent constant—CGColorRenderingIntent.defaultIntent, CGColorRenderingIntent.absoluteColorimetric, CGColorRenderingIntent.relativeColorimetric, CGColorRenderingIntent.perceptual, or CGColorRenderingIntent.saturation. For a discussion of these constants, see CGColorSpace.

## Discussion

The rendering intent specifies how to handle colors that are not located within the gamut of the destination color space of a graphics context. If you do not explicitly set the rendering intent, Core Graphics uses perceptual rendering intent when drawing sampled images and relative colorimetric rendering intent for all other drawing.

## See Also

### Managing a Graphics Context

func flush()

Forces all pending drawing operations in a window context to be rendered immediately to the destination device.

func synchronize()

Marks a window context for update.

func setBlendMode(CGBlendMode)

Sets how sample values are composited by a graphics context.

enum CGBlendMode

Compositing operations for images.

