

- Spatial
- Angle2D
-  init(degrees:) 

Initializer

# init(degrees:)

Creates an angle with the specified floating-point degrees.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(degrees: T) where T : BinaryFloatingPoint
```

## Parameters 

`degrees`  

A floating-point value that specifies the angle in degrees.

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

init&lt;T>(radians: T)

Creates an angle with the specified floating-point radians.

init(degrees: Double)

Creates an angle with the specified double-precision degrees.

static func degrees(Double) -> Angle2D

Returns a new angle structure with the specified double-precision degrees.

static func radians(Double) -> Angle2D

Returns a new angle structure with the specified double-precision radians.

