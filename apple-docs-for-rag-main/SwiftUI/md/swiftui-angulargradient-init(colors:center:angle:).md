

- SwiftUI
- AngularGradient
-  init(colors:center:angle:) 

Initializer

# init(colors:center:angle:)

Creates a conic gradient from a collection of colors that completes a full turn.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    colors: [Color],
    center: UnitPoint,
    angle: Angle = .zero
)
```

## See Also

### Creating a full rotation angular gradient

init(gradient: Gradient, center: UnitPoint, angle: Angle)

Creates a conic gradient that completes a full turn.

init(stops: [Gradient.Stop], center: UnitPoint, angle: Angle)

Creates a conic gradient from a collection of color stops that completes a full turn.

