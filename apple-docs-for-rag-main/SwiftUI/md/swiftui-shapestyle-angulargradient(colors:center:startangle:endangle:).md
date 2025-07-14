

- SwiftUI
- ShapeStyle
-  angularGradient(colors:center:startAngle:endAngle:) 

Type Method

# angularGradient(colors:center:startAngle:endAngle:)

An angular gradient defined by a collection of colors.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func angularGradient(
    colors: [Color],
    center: UnitPoint,
    startAngle: Angle,
    endAngle: Angle
) -> AngularGradient
```

Available when `Self` is `AngularGradient`.

## Parameters 

`colors`  

The colors of the gradient, evenly spaced along its full length.

`center`  

The relative center of the gradient, mapped from the unit space into the bounding rectangle of the filled shape.

`startAngle`  

The angle that marks the beginning of the gradient.

`endAngle`  

The angle that marks the end of the gradient.

## Discussion

For more information on how to use angular gradients, see angularGradient(_:center:startAngle:endAngle:).

## See Also

### Angular gradients

static angularGradient(_:center:startAngle:endAngle:)

An angular gradient, which applies the color function as the angle changes between the start and end angles, and anchored to a relative center point within the filled shape.

static func angularGradient(stops: [Gradient.Stop], center: UnitPoint, startAngle: Angle, endAngle: Angle) -> AngularGradient

An angular gradient defined by a collection of color stops.

