

- SwiftUI
- ShapeStyle
-  radialGradient(stops:center:startRadius:endRadius:) 

Type Method

# radialGradient(stops:center:startRadius:endRadius:)

A radial gradient defined by a collection of color stops.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func radialGradient(
    stops: [Gradient.Stop],
    center: UnitPoint,
    startRadius: CGFloat,
    endRadius: CGFloat
) -> RadialGradient
```

Available when `Self` is `RadialGradient`.

## Discussion

The gradient applies the color function as the distance from a center point, scaled to fit within the defined start and end radii. The gradient maps the unit space center point into the bounding rectangle of each shape filled with the gradient.

For information about how to use shape styles, see ShapeStyle.

## See Also

### Radial gradients

static radialGradient(_:center:startRadius:endRadius:)

A radial gradient.

static func radialGradient(colors: [Color], center: UnitPoint, startRadius: CGFloat, endRadius: CGFloat) -> RadialGradient

A radial gradient defined by a collection of colors.

