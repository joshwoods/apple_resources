

- Core Graphics
- CGContext
-  drawRadialGradient(\_:startCenter:startRadius:endCenter:endRadius:options:) 

Instance Method

# drawRadialGradient(\_:startCenter:startRadius:endCenter:endRadius:options:)

Paints a gradient fill that varies along the area defined by the provided starting and ending circles.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func drawRadialGradient(
    _ gradient: CGGradient,
    startCenter: CGPoint,
    startRadius: CGFloat,
    endCenter: CGPoint,
    endRadius: CGFloat,
    options: CGGradientDrawingOptions
)
```

## Parameters 

`gradient`  

A CGGradient object.

`startCenter`  

The coordinate that defines the center of the starting circle.

`startRadius`  

The radius of the starting circle.

`endCenter`  

The coordinate that defines the center of the ending circle.

`endRadius`  

The radius of the ending circle.

`options`  

Option flags (drawsBeforeStartLocation or drawsAfterEndLocation) that control whether the gradient is drawn before the starting circle or after the ending circle.

## Discussion

The color at location 0 in the CGGradient object is mapped to the circle defined by `startCenter` and `startRadius`. The color at location 1 in the CGGradient object is mapped to the circle defined by `endCenter` and `endRadius`. Colors are linearly interpolated between the starting and ending circles based on the location values of the gradient. The option flags control whether the gradient is drawn before the start point or after the end point.

## See Also

### Drawing Gradients and Shadings

func drawLinearGradient(CGGradient, start: CGPoint, end: CGPoint, options: CGGradientDrawingOptions)

Paints a gradient fill that varies along the line defined by the provided starting and ending points.

struct CGGradientDrawingOptions

Drawing locations for gradients.

func drawShading(CGShading)

Fills the clipping path of a context with the specified shading.

