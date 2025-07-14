

- SwiftUI
- ShapeStyle
-  radialGradient(\_:center:startRadius:endRadius:) 

Type Method

# radialGradient(\_:center:startRadius:endRadius:)

A radial gradient.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func radialGradient(
    _ gradient: AnyGradient,
    center: UnitPoint = .center,
    startRadius: CGFloat = 0,
    endRadius: CGFloat
) -> some ShapeStyle
```

Available when `Self` is `RadialGradient`.

Show all declarations

## Discussion

The gradient applies the color function as the distance from a center point, scaled to fit within the defined start and end radii. The gradient maps the unit space center point into the bounding rectangle of each shape filled with the gradient.

For example, a radial gradient used as a background:

```
ContentView()
    .background(.radialGradient(.red.gradient, endRadius: 100))
```

For information about how to use shape styles, see ShapeStyle.

## See Also

### Radial gradients

static func radialGradient(colors: [Color], center: UnitPoint, startRadius: CGFloat, endRadius: CGFloat) -> RadialGradient

A radial gradient defined by a collection of colors.

static func radialGradient(stops: [Gradient.Stop], center: UnitPoint, startRadius: CGFloat, endRadius: CGFloat) -> RadialGradient

A radial gradient defined by a collection of color stops.

