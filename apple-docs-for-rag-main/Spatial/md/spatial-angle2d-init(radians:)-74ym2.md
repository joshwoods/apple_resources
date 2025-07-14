

- Spatial
- Angle2D
-  init(radians:) 

Initializer

# init(radians:)

Creates an angle with the specified floating-point radians.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(radians: T) where T : BinaryFloatingPoint
```

## Parameters 

`radians`  

A floating-point value that specifies the angle in radians.

## See Also

### Creating an angle structure

init()

Creates an angle.

init(Angle)

Creates an angle from a SwiftUI angle.

init(radians: Double)

Creates an angle with the specified double-precision radians.

init(radians: Double)

Creates an angle with the specified double-precision radians.

init&lt;T>(degrees: T)

Creates an angle with the specified floating-point degrees.

init(degrees: Double)

Creates an angle with the specified double-precision degrees.

static func degrees(Double) -> Angle2D

Returns a new angle structure with the specified double-precision degrees.

static func radians(Double) -> Angle2D

Returns a new angle structure with the specified double-precision radians.

