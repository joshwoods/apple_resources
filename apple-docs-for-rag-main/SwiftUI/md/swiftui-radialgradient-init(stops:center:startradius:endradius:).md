

- SwiftUI
- RadialGradient
-  init(stops:center:startRadius:endRadius:) 

Initializer

# init(stops:center:startRadius:endRadius:)

Creates a radial gradient from a collection of color stops.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    stops: [Gradient.Stop],
    center: UnitPoint,
    startRadius: CGFloat,
    endRadius: CGFloat
)
```

## See Also

### Creating a radial gradient

init(gradient: Gradient, center: UnitPoint, startRadius: CGFloat, endRadius: CGFloat)

Creates a radial gradient from a base gradient.

init(colors: [Color], center: UnitPoint, startRadius: CGFloat, endRadius: CGFloat)

Creates a radial gradient from a collection of colors.

