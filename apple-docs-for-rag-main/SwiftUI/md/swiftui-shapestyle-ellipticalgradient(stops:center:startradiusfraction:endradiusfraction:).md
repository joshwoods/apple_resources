

- SwiftUI
- ShapeStyle
-  ellipticalGradient(stops:center:startRadiusFraction:endRadiusFraction:) 

Type Method

# ellipticalGradient(stops:center:startRadiusFraction:endRadiusFraction:)

A radial gradient that draws an ellipse defined by a collection of color stops.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func ellipticalGradient(
    stops: [Gradient.Stop],
    center: UnitPoint = .center,
    startRadiusFraction: CGFloat = 0,
    endRadiusFraction: CGFloat = 0.5
) -> EllipticalGradient
```

Available when `Self` is `EllipticalGradient`.

## Discussion

The gradient maps its coordinate space to the unit space square in which its center and radii are defined, then stretches that square to fill its bounding rect, possibly also stretching the circular gradient to have elliptical contours.

For example, an elliptical gradient used as a background:

```
.background(.ellipticalGradient(stops: [
    .init(color: .red, location: 0.0),
    .init(color: .yellow, location: 0.9),
    .init(color: .yellow, location: 1.0),
]))
```

For information about how to use shape styles, see ShapeStyle.

## See Also

### Elliptical gradients

static ellipticalGradient(_:center:startRadiusFraction:endRadiusFraction:)

A radial gradient that draws an ellipse.

static func ellipticalGradient(colors: [Color], center: UnitPoint, startRadiusFraction: CGFloat, endRadiusFraction: CGFloat) -> EllipticalGradient

A radial gradient that draws an ellipse defined by a collection of colors.

