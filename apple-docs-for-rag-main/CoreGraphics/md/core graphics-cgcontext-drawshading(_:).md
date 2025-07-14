

- Core Graphics
- CGContext
-  drawShading(\_:) 

Instance Method

# drawShading(\_:)

Fills the clipping path of a context with the specified shading.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func drawShading(_ shading: CGShading)
```

## Parameters 

`shading`  

A shading object. The shading object is retained; upon return, you may safely release it.

## Discussion

The preferred way to draw gradients is to use a CGGradient object. See CGGradient.

## See Also

### Related Documentation

func drawRadialGradient(CGGradient, startCenter: CGPoint, startRadius: CGFloat, endCenter: CGPoint, endRadius: CGFloat, options: CGGradientDrawingOptions)

Paints a gradient fill that varies along the area defined by the provided starting and ending circles.

func drawLinearGradient(CGGradient, start: CGPoint, end: CGPoint, options: CGGradientDrawingOptions)

Paints a gradient fill that varies along the line defined by the provided starting and ending points.

### Drawing Gradients and Shadings

func drawLinearGradient(CGGradient, start: CGPoint, end: CGPoint, options: CGGradientDrawingOptions)

Paints a gradient fill that varies along the line defined by the provided starting and ending points.

func drawRadialGradient(CGGradient, startCenter: CGPoint, startRadius: CGFloat, endCenter: CGPoint, endRadius: CGFloat, options: CGGradientDrawingOptions)

Paints a gradient fill that varies along the area defined by the provided starting and ending circles.

struct CGGradientDrawingOptions

Drawing locations for gradients.

