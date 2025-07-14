

- SwiftUI
- ShapeStyle
-  angularGradient(\_:center:startAngle:endAngle:) 

Type Method

# angularGradient(\_:center:startAngle:endAngle:)

An angular gradient, which applies the color function as the angle changes between the start and end angles, and anchored to a relative center point within the filled shape.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func angularGradient(
    _ gradient: AnyGradient,
    center: UnitPoint = .center,
    startAngle: Angle,
    endAngle: Angle
) -> some ShapeStyle
```

Available when `Self` is `AngularGradient`.

Show all declarations

## Parameters 

`gradient`  

The gradient to use for filling the shape, providing the colors and their relative stop locations.

`center`  

The relative center of the gradient, mapped from the unit space into the bounding rectangle of the filled shape.

`startAngle`  

The angle that marks the beginning of the gradient.

`endAngle`  

The angle that marks the end of the gradient.

## Discussion

An angular gradient is also known as a “conic” gradient. If `endAngle - startAngle > 2π`, the gradient only draws the last complete turn. If `endAngle - startAngle 

```
ContentView()
    .background(.angularGradient(.red.gradient))
```

For information about how to use shape styles, see ShapeStyle.

## See Also

### Angular gradients

static func angularGradient(colors: [Color], center: UnitPoint, startAngle: Angle, endAngle: Angle) -> AngularGradient

An angular gradient defined by a collection of colors.

static func angularGradient(stops: [Gradient.Stop], center: UnitPoint, startAngle: Angle, endAngle: Angle) -> AngularGradient

An angular gradient defined by a collection of color stops.

