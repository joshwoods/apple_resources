

- SwiftUI
- PhysicalMetricsConverter
-  convert(\_:to:) 

Instance Method

# convert(\_:to:)

Converts a point’s coordinates to physical length measurements in the specified unit.

visionOS 1.0+

``` source
@MainActor @preconcurrency
func convert(
    _ point: CGPoint,
    to unit: UnitLength
) -> CGPoint
```

Show all declarations

## Return Value

A point value with physical length measurements, in the given unit

## Discussion

The point is assumed to be in the coordinate system of the scene that this converter is associated with. If the scene is scaled, the physical measurement will take this scale into account.

## See Also

### Converting a unit length

func convert(_:from:)

Converts a length in the specified unit to a length in points suitable for use in the environment this converter is associated with.

