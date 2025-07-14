

- SwiftUI
- ShapeStyle
-  conicGradient(stops:center:angle:) 

Type Method

# conicGradient(stops:center:angle:)

A conic gradient defined by a collection of color stops that completes a full turn.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func conicGradient(
    stops: [Gradient.Stop],
    center: UnitPoint,
    angle: Angle = .zero
) -> AngularGradient
```

Available when `Self` is `AngularGradient`.

## Parameters 

`stops`  

The color stops of the gradient, defining each component color and their relative location along the gradient’s full length.

`center`  

The relative center of the gradient, mapped from the unit space into the bounding rectangle of the filled shape.

`angle`  

The angle to offset the beginning of the gradient’s full turn.

## Discussion

For more information on how to use conic gradients, see conicGradient(_:center:angle:).

## See Also

### Conic gradients

static conicGradient(_:center:angle:)

A conic gradient that completes a full turn, optionally starting from a given angle and anchored to a relative center point within the filled shape.

static func conicGradient(colors: [Color], center: UnitPoint, angle: Angle) -> AngularGradient

A conic gradient defined by a collection of colors that completes a full turn.

