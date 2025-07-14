

- SwiftUI
- ShapeStyle
-  linearGradient(colors:startPoint:endPoint:) 

Type Method

# linearGradient(colors:startPoint:endPoint:)

A linear gradient defined by a collection of colors.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func linearGradient(
    colors: [Color],
    startPoint: UnitPoint,
    endPoint: UnitPoint
) -> LinearGradient
```

Available when `Self` is `LinearGradient`.

## Discussion

The gradient applies the color function along an axis, as defined by its start and end points. The gradient maps the unit space points into the bounding rectangle of each shape filled with the gradient.

For information about how to use shape styles, see ShapeStyle.

## See Also

### Linear gradients

static linearGradient(_:startPoint:endPoint:)

A linear gradient.

static func linearGradient(stops: [Gradient.Stop], startPoint: UnitPoint, endPoint: UnitPoint) -> LinearGradient

A linear gradient defined by a collection of color stops.

