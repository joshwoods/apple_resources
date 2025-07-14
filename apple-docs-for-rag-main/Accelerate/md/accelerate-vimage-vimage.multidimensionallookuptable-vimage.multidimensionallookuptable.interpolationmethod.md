

- Accelerate
- vImage
- vImage.MultidimensionalLookupTable
-  vImage.MultidimensionalLookupTable.InterpolationMethod 

Enumeration

# vImage.MultidimensionalLookupTable.InterpolationMethod

Describes the method a multidimensional lookup table uses the generate interpolated values between lookup table values.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
enum InterpolationMethod
```

## Topics

### Enumeration Cases

case full

Full linear interpolation.

case half

Partial linear interpolation between vertices on gray axis and `N-1` nearest vertices.

case none

Nearest neighbor.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

