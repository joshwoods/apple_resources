

- SwiftUI
- PhysicalMetricsConverter
-  convert(\_:from:) 

Instance Method

# convert(\_:from:)

Converts a length in the specified unit to a length in points suitable for use in the environment this converter is associated with.

visionOS 1.0+

``` source
@MainActor @preconcurrency
func convert(
    _ lengthValue: CGFloat,
    from unit: UnitLength
) -> CGFloat
```

Show all declarations

## Return Value

A value in points. Use this value only in the scene this converter was associated with.

## See Also

### Converting a unit length

func convert(_:to:)

Converts a point’s coordinates to physical length measurements in the specified unit.

