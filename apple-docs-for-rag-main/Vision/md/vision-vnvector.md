

- Vision
-  VNVector 

Class

# VNVector

An immutable 2D vector represented by its x-axis and y-axis projections.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class VNVector
```

## Topics

### Creating a Vector

init(byAdding: VNVector, to: VNVector)

Creates a new vector by adding the specified vectors.

init(bySubtracting: VNVector, from: VNVector)

Creates a new vector by subtracting the first vector from the second vector.

init(byMultiplying: VNVector, byScalar: Double)

Creates a new vector by multiplying the specified vector’s x-axis and y-axis projections by the scalar value.

convenience init(r: Double, theta: Double)

Creates a new vector in polar coordinate space.

convenience init(vectorHead: VNPoint, tail: VNPoint)

Creates a new vector in Cartesian coordinate space.

init(xComponent: Double, yComponent: Double)

Creates a new vector in Cartesian coordinate space, based on its x-axis and y-axis projections.

class var zero: VNVector

A vector object with zero length.

### Inspecting a Vector

var length: Double

The length, or absolute value, of the vector.

var r: Double

The radius, absolute value, or length of the vector.

var theta: Double

The angle between the vector direction and the positive direction of the x-axis.

var squaredLength: Double

The squared length of the vector.

var x: Double

A signed projection that indicates the vector’s direction on the x-axis.

var y: Double

A signed projection that indicates the vector’s direction on the y-axis.

class func dotProduct(of: VNVector, vector: VNVector) -> Double

Caclulates the dot product of two vectors.

class func unitVector(for: VNVector) -> VNVector

Calculates a vector that’s normalized by preserving its direction, so that the vector length equals 1.0.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Common data types

class VNCircle

An immutable 2D circle represented by its center point and radius.

