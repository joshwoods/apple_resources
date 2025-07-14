

- Vision
- VNVector
-  length 

Instance Property

# length

The length, or absolute value, of the vector.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var length: Double { get }
```

## See Also

### Inspecting a Vector

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

