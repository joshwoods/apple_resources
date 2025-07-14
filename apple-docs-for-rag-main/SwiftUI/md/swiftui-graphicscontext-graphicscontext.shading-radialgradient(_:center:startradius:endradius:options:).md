

- SwiftUI
- GraphicsContext
- GraphicsContext.Shading
-  radialGradient(\_:center:startRadius:endRadius:options:) 

Type Method

# radialGradient(\_:center:startRadius:endRadius:options:)

Returns a shading instance that fills a radial gradient.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func radialGradient(
    _ gradient: Gradient,
    center: CGPoint,
    startRadius: CGFloat,
    endRadius: CGFloat,
    options: GraphicsContext.GradientOptions = GradientOptions()
) -> GraphicsContext.Shading
```

## Parameters 

`gradient`  

A Gradient instance that defines the colors of the gradient.

`center`  

The point in the current user space on which SwiftUI centers the gradient.

`startRadius`  

The distance from the center where the gradient starts.

`endRadius`  

The distance from the center where the gradient ends.

`options`  

Options that you use to configure the gradient.

## Return Value

A shading instance filled with a radial gradient.

## See Also

### Gradients

static func linearGradient(Gradient, startPoint: CGPoint, endPoint: CGPoint, options: GraphicsContext.GradientOptions) -> GraphicsContext.Shading

Returns a shading instance that fills a linear (axial) gradient.

static func conicGradient(Gradient, center: CGPoint, angle: Angle, options: GraphicsContext.GradientOptions) -> GraphicsContext.Shading

Returns a shading instance that fills a conic (angular) gradient.

