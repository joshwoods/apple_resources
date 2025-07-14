

- SwiftUI
- ShapeStyle
-  linearGradient(\_:startPoint:endPoint:) 

Type Method

# linearGradient(\_:startPoint:endPoint:)

A linear gradient.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func linearGradient(
    _ gradient: AnyGradient,
    startPoint: UnitPoint,
    endPoint: UnitPoint
) -> some ShapeStyle
```

Available when `Self` is `LinearGradient`.

Show all declarations

## Discussion

The gradient applies the color function along an axis, as defined by its start and end points. The gradient maps the unit space points into the bounding rectangle of each shape filled with the gradient.

For example, a linear gradient used as a background:

```
ContentView()
    .background(.linearGradient(.red.gradient,
        startPoint: .top, endPoint: .bottom))
```

For information about how to use shape styles, see ShapeStyle.

## See Also

### Linear gradients

static func linearGradient(colors: [Color], startPoint: UnitPoint, endPoint: UnitPoint) -> LinearGradient

A linear gradient defined by a collection of colors.

static func linearGradient(stops: [Gradient.Stop], startPoint: UnitPoint, endPoint: UnitPoint) -> LinearGradient

A linear gradient defined by a collection of color stops.

