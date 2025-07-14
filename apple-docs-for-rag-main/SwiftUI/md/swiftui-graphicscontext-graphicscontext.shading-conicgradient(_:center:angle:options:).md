

- SwiftUI
- GraphicsContext
- GraphicsContext.Shading
-  conicGradient(\_:center:angle:options:) 

Type Method

# conicGradient(\_:center:angle:options:)

Returns a shading instance that fills a conic (angular) gradient.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func conicGradient(
    _ gradient: Gradient,
    center: CGPoint,
    angle: Angle = Angle(),
    options: GraphicsContext.GradientOptions = GradientOptions()
) -> GraphicsContext.Shading
```

## Parameters 

`gradient`  

A Gradient instance that defines the colors of the gradient.

`center`  

The point in the current user space on which SwiftUI centers the gradient.

`angle`  

The angle about the center that SwiftUI uses to start and finish the gradient. The gradient sweeps all the way around the center.

`options`  

Options that you use to configure the gradient.

## Return Value

A shading instance filled with a conic gradient.

## See Also

### Gradients

static func linearGradient(Gradient, startPoint: CGPoint, endPoint: CGPoint, options: GraphicsContext.GradientOptions) -> GraphicsContext.Shading

Returns a shading instance that fills a linear (axial) gradient.

static func radialGradient(Gradient, center: CGPoint, startRadius: CGFloat, endRadius: CGFloat, options: GraphicsContext.GradientOptions) -> GraphicsContext.Shading

Returns a shading instance that fills a radial gradient.

