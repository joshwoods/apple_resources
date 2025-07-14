

- SwiftUI
- PhysicalMetric
-  init(wrappedValue:from:) 

Initializer

# init(wrappedValue:from:)

Creates a value that maps the specified point, whose dimensions are specified in physical length measurements in the given unit, to the corresponding value in points in the associated scene.

visionOS 1.0+

``` source
init(
    wrappedValue point: CGPoint,
    from unit: UnitLength
) where Value == CGPoint
```

Show all declarations

